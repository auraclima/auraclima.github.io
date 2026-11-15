# DOSSIÊ TÉCNICO E DECLARAÇÃO FORMAL DE AUTORIA DE SOFTWARE

**PROGRAMA DE COMPUTADOR:** AURA CLIMA  
**SUBTÍTULO:** Meteorologia em Tempo Real & Planejamento de Rotas com GPS  
**VERSÃO DA OBRA:** 1.0.0  
**DATA DE CONCLUSÃO:** Outubro/Novembro de 2026  
**REGIME JURÍDICO:** Lei nº 9.609/1998 (Proteção da Propriedade Intelectual de Programa de Computador) e Lei nº 9.610/1998 (Direitos Autorais)  
**DOMÍNIO OFICIAL PÚBLICO:** https://auraclima.github.io/  
**REPOSITÓRIO DE CÓDIGO:** https://github.com/auraclima/auraclima.github.io  

---

## 1. DADOS DO AUTOR E TITULAR DOS DIREITOS
*(Preencha os dados abaixo ao submeter para o Selo de Autoria / INPI)*

- **Nome Completo do Autor:** __________________________________________________
- **CPF / CNPJ:** ______________________________________________________________
- **E-mail:** __________________________________________________________________
- **Nacionalidade:** Brasileira
- **País de Criação:** Brasil
- **Natureza da Titularidade:** Autor Original e Criador Único do Código-Fonte

---

## 2. DADOS CADASTRAIS DO SOFTWARE (PADRÃO INPI / SELO DE AUTORIA)

- **Título do Programa de Computador:** AURA CLIMA
- **Tipo de Programa:** Software Aplicativo / Sistema Web & Mobile PWA (Progressive Web App)
- **Campo de Aplicação:** Meteorologia, Previsão do Tempo, Roteirização Rodoviária e Navegação GPS (Código INPI: UT-01 / TC-01)
- **Linguagens de Programação:** JavaScript (ECMAScript 6+ Vanilla), HTML5, CSS3, SVG, JSON
- **Arquitetura de Execução:** Frontend Client-Side puro e autônomo, sem necessidade de servidores backend dedicados para o usuário, integrando APIs abertas e descentralizadas.
- **Sistemas Operacionais Suportados:** Multiplataforma (Windows, Android, iOS, iPadOS, macOS, Linux) compatível com todos os navegadores modernos com suporte a W3C e PWA.

---

## 3. RESUMO CRIPTOGRÁFICO OFICIAL (HASHES DE ANTERIORIDADE)

O código-fonte integral deste programa encontra-se empacotado no arquivo **`AuraClima_CodigoFonte.zip`**, cujo resumo criptográfico imutável atesta sua anterioridade e integridade:

- **Algoritmo SHA-512 (Padrão Oficial INPI):**
  `640e74a3941e22ed98b79d8e22cace4d7af0ee6dc3a688bec332b5bc91e0810deb68ca6938488b62cd37e906728aa4e7dd01f238960ec9d1d851937ba78fec6e`

- **Algoritmo SHA-256 (Padrão Blockchain / Selo RFC 3161):**
  `dbd5e4d5d8f57209750c13970eb26cb8274dc3991f4d6a6569d79defa2bcc16b`

- **Tamanho do Arquivo Compactado:** 50478 bytes

### 3.1. Certificação Registrada no Selo de Autoria
- **Identificador de Registro (ID):** `SA-20261115-1DDF473C`
- **Link Oficial de Verificação Pública:** https://selo-de.autoria-tech.workers.dev/?verify=SA-20261115-1DDF473C
- **Badge de Autoria:** `[![Selo de Autoria](https://img.shields.io/badge/Selo_de_Autoria-SA--20261115--1DDF473C-0891b2)](https://selo-de.autoria-tech.workers.dev/?verify=SA-20261115-1DDF473C)`

---

## 4. MEMORIAL DESCRITIVO E INOVAÇÕES TÉCNICAS

O **Aura Clima** é um software de meteorologia e navegação que une previsão do tempo de alta precisão a um planejador de viagens integrado a mapas e GPS em tempo real. As principais soluções técnicas criadas incluem:

### 4.1. Módulo Meteorológico em Tempo Real (`js/api.js` e `js/weather-codes.js`)
- Mecanismo autônomo de busca de cidades global com autocomplete inteligente e classificação por relevância e bandeiras de países.
- Consumo direto e sem chave de API da Open-Meteo API, realizando cálculos de sensação térmica, umidade, vento com bússola vetorial dinâmica, ponto de orvalho, pressão atmosférica, visibilidade, radiação UV e índice europeu de qualidade do ar (AQI).
- Cálculo astronômico preciso da fase lunar (Nova, Crescente, Cheia, Minguante) e porcentagem de iluminação.
- Sistema de alertas meteorológicos preditivos baseado em códigos WMO (tempestades, chuvas torrenciais, ventos fortes e calor/frio extremo).

### 4.2. Planejador Rodoviário & Traçado com GPS (`js/route-planner.js`)
- Algoritmo que calcula traçado rodoviário real de estradas conectando Origem e Destino via motor de roteirização OSRM, calculando quilometragem exata e duração estimada da viagem.
- Renderização em mapa interativo multi-camada através da biblioteca Leaflet (com alternância entre OpenStreetMap, Satélite Real ESRI, Rodovias e Modo Noturno).
- Mapeamento inteligente de condições de estrada (risco de aquaplanagem, pista molhada, neblina na serra ou tempestades no destino).
- Projeção meteorológica dia a dia no destino para o período exato de estadia escolhido pelo usuário (1 a 7 dias).
- Exportador de rotas universal no formato `.GPX` compatível com dispositivos automotivos, Garmin, OsmAnd e Strava.
- Modo Viagem em Tempo Real com rastreamento GPS contínuo (`navigator.geolocation.watchPosition`), velocímetro digital (km/h) e cálculo de distância restante até a chegada.

### 4.3. Sistema de Compartilhamento Dinâmico em Redes e Rotas por URL
- Mecanismo que empacota os dados da viagem ou da cidade em parâmetros de URL (`?tab=route&o=...&d=...&days=...`), permitindo que outro usuário abra o link e veja a rota desenhada no mapa e a previsão sem precisar digitar nada.
- Integração de compartilhamento em 1 clique para WhatsApp, Telegram, X (Twitter), Facebook e Web Share API nativa.

### 4.4. Interface Reativa & Motor de Partículas em Canvas (`index.html`, `css/style.css`, `js/app.js`)
- Motor gráfico em HTML5 Canvas de alto desempenho renderizando partículas dinâmicas (gotas de chuva, flocos de neve, poeira de sol e estrelas cintilantes) que reagem ao clima e ao horário (dia/noite).
- Alternância instantânea de visualização horária entre Carrossel de Cards e Gráfico SVG com curvas bezier suaves e gradientes térmicos.
- Design moderno com Glassmorphism, paleta aeroespacial e responsividade total para celulares, tablets e computadores.

### 4.5. Arquitetura PWA e Resiliência Offline (`sw.js` e `manifest.json`)
- Service Worker que gerencia cache de ativos estáticos permitindo que a aplicação abra instantaneamente mesmo sem conexão com a internet.
- Suporte a instalação nativa na tela inicial (Home Screen) do Android, Windows e iOS.

---

## 5. DECLARAÇÃO FORMAL DE VERACIDADE E AUTORIA

Declaro sob as penas da lei, em especial o Art. 299 do Código Penal Brasileiro e os termos da Lei nº 9.609/1998, que:

1. Sou o legítimo autor, idealizador e desenvolvedor do programa de computador denominado **AURA CLIMA**.
2. O código-fonte compactado no arquivo `AuraClima_CodigoFonte.zip` corresponde com exatidão à versão criada por mim.
3. Não utilizei de plágio ou cópia desautorizada de terceiros na elaboração da lógica proprietária desta obra intelectual.
4. Os dados apresentados neste dossiê e o resumo criptográfico acima são a fiel expressão da verdade.

Local: ____________________________, Data: ____ de ________________ de 2026.

___________________________________________________________  
**Assinatura do Autor / Titular**  
*(ou Assinatura com Certificado Digital ICP-Brasil / Gov.br)*
