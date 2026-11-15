# GUIA PRÁTICO: COMO REGISTRAR O AURA CLIMA NO SELO DE AUTORIA E NO INPI

Este documento explica os passos exatos para formalizar a proteção do seu software **Aura Clima**.

---

## OPÇÃO 1: REGISTRO VIA SELO DE AUTORIA (Avctoris / Blockchain / Carimbo do Tempo)
*Método rápido (leva menos de 10 minutos), com validade jurídica em mais de 170 países pela Convenção de Berna.*

1. **Acesse uma plataforma de Selo de Autoria credenciada:**
   - **Avctoris:** [https://www.avctoris.com/](https://www.avctoris.com/) (muito utilizada no Brasil para registro de código e obras intelectuais)
   - Ou outra plataforma de registro de autoria com carimbo do tempo ICP-Brasil / Blockchain (ex: Autoria Fácil, OriginalMy).
2. **Faça o cadastro ou login** na plataforma.
3. **Selecione a opção:** "Registrar Obra" / "Registro de Software / Código-Fonte".
4. **Envio do Arquivo:**
   - Faça o upload do arquivo: **`AuraClima_CodigoFonte.zip`** (localizado nesta pasta).
   - Como documento complementar (se solicitado), anexe o arquivo **`DOSSIE_DECLARACAO_DE_AUTORIA.md`** ou o **`HASHES_CRIPTOGRAFICOS.txt`**.
5. **Preencha os dados do Software:**
   - **Título da Obra:** Aura Clima
   - **Tipo de Obra:** Software / Programa de Computador
   - **Autor:** Seu nome completo e CPF
6. **Conclusão:**
   - A plataforma irá gerar o **Certificado de Registro de Autoria** com Carimbo do Tempo oficial (RFC 3161) e o Selo de Autoria com QR Code e Hash SHA-256.
   - Guarde esse certificado em PDF, pois ele é a sua prova pública de anterioridade mundial!

---

## OPÇÃO 2: REGISTRO OFICIAL NO INPI (Instituto Nacional da Propriedade Industrial)
*Órgão oficial do Governo Brasileiro (validade de 50 anos, indispensável para editais públicos e licitações).*

1. **Emitir e Pagar a GRU (Guia de Recolhimento da União):**
   - Acesse o portal do INPI: [https://gru.inpi.gov.br/](https://gru.inpi.gov.br/)
   - Selecione a unidade: **Programas de Computador**.
   - Serviço: **Pedido de Registro de Programa de Computador** (Código **661**).
   - Valor: Taxa com desconto para pessoa física / MEI / ME. Pague a guia e guarde o "Nosso Número".
2. **Acessar o sistema e-Software do INPI:**
   - Acesse com sua conta gov.br ou login do INPI: [https://sistema.inpi.gov.br/](https://sistema.inpi.gov.br/)
   - Digite o número da GRU paga.
3. **Preencher o Formulário:**
   - **Título:** Aura Clima
   - **Linguagens:** JavaScript, HTML5, CSS3
   - **Campo de Aplicação:** Meteorologia / Transporte / Sistemas de Informação (UT-01)
   - **Tipo de Programa:** Software Aplicativo (TC-01)
4. **Inserir o Hash SHA-512 (Obrigatório):**
   - O INPI não aceita upload do código fonte em texto, ele pede **apenas o Hash SHA-512 do ZIP**.
   - Copie o hash abaixo (que consta no arquivo `HASHES_CRIPTOGRAFICOS.txt`):
   ```
   640e74a3941e22ed98b79d8e22cace4d7af0ee6dc3a688bec332b5bc91e0810deb68ca6938488b62cd37e906728aa4e7dd01f238960ec9d1d851937ba78fec6e
   ```
5. **Assinar a Declaração de Veracidade (DV):**
   - O sistema gerará o PDF da DV.
   - Assine digitalmente com seu **Certificado Digital ICP-Brasil** (e-CPF) ou conforme as instruções vigentes do INPI.
   - Envie o arquivo assinado no portal.
6. **Pronto!** Em cerca de 7 a 10 dias úteis, o INPI emite o **Certificado Oficial de Registro de Programa de Computador**.

---

## 📁 O QUE HÁ NESTA PASTA PARA VOCÊ GUARDAR:

1. **`AuraClima_CodigoFonte.zip`**: Código-fonte original e puro empacotado. **NÃO altere nem renomeie este arquivo**, pois qualquer alteração mudará o Hash criptográfico!
2. **`DOSSIE_DECLARACAO_DE_AUTORIA.md`**: Memorial descritivo formal com dados do software e declaração de autoria.
3. **`HASHES_CRIPTOGRAFICOS.txt`**: Tabela com os resumos SHA-512 e SHA-256 de todos os arquivos.
4. **`codigo-fonte/`**: Pasta aberta com os arquivos para você consultar a qualquer momento.
5. **`PACOTE_COMPLETO_REGISTRO_AURA_CLIMA.zip`**: Pacote consolidado contendo todos os itens acima juntos.
