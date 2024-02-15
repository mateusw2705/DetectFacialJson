# Tutorial: Laboratorio de Teste de Deteccao de Imagem no Azure

Este tutorial irá guia-lo através do processo de usar o laboratório de teste de detecção de imagem no Azure e interpretar o JSON retornado.

## Pré-requisitos

- Conta no Azure com acesso ao serviço de detecção de imagem
- Conhecimento basico de manipulação de JSON

## Passo 1: Acessar o Serviço de Deteccção de Imagem no Azure

1. Faça login na sua conta do Azure.
2. Navegue até o serviço de detecção de imagem.

## Passo 2: Realizar o Teste de Detecção de Imagem

1. Faça o upload da imagem que você deseja testar.
2. Aguarde o processamento.
3. O resultado será retornado no formato JSON.

4. 
![Capturar](https://github.com/mateusw2705/DetectFacialJson/assets/112732200/aae97c71-f78c-45e6-900a-92f358c42ad6)"




## Passo 3: Interpretar o JSON Retornado

O JSON retornado conterá informações sobre a detecção de objetos na imagem. Aqui está um exemplo de como o JSON pode ser estruturado:

```json
{
  "apim-request-id": "2d061009-a093-4ca8-a2af-22d7b79bef73",
  "comprimento do conteúdo": "1263",
  "content-type": "aplicativo/json; charset=utf-8",
  "modelVersion": "2023-10-01",
  "denseCaptionsResult": {
    "valores": [
      {
        "texto": "uma mulher com as mãos no rosto",
        "confiança": 0,7922150492668152,
        "boundingBox": {
          "x": 0,
          "s": 0,
          "w": 2000,
          "h": 2999
        }
      },
      {
        "texto": "uma mulher com as mãos no rosto",
        "confiança": 0,7960794568061829,
        "boundingBox": {
          "x": 32,
          "s": 189,
          "w": 1907,
          "h": 2760
        }
      },
      {
        "texto": "close da boca e dos dentes de uma pessoa",
        "confiança": 0,7925179600715637,
        "boundingBox": {
          "x": 836,
          "s": 1226,
          "w": 404,
          "h": 186
        }
      },
      {
        "texto": "close dos olhos e sobrancelhas de uma pessoa",
        "confiança": 0,8013100624084473,
        "boundingBox": {
          "x": 678,
          "s": 823,
          "w": 723,
          "h": 302
        }
      },
      {
        "texto": "uma mulher sorrindo com as mãos no rosto",
        "confiança": 0,8066269755363464,
        "boundingBox": {
          "x": 561,
          "s": 185,
          "w": 1005,
          "h": 1459
        }
      },
      {
        "texto": "close dos dentes de uma pessoa",
        "confiança": 0,808774471282959,
        "boundingBox": {
          "x": 866,
          "s": 1251,
          "w": 346,
          "h": 108
        }
      },
      {
        "text": "close do nariz de uma pessoa e do nariz usando óculos",
        "confiança": 0,839764416217804,
        "boundingBox": {
          "x": 941,
          "s": 970,
          "w": 208,
          "h": 219
        }
      },
      {
        "texto": "um close do rosto de uma mulher",
        "confiança": 0,8797226548194885,
        "boundingBox": {
          "x": 583,
          "s": 215,
          "w": 873,
          "h": 748
        }
      },
      {
        "texto": "um close-up do olho de uma pessoa",
        "confiança": 0,9100437164306641,
        "boundingBox": {
          "x": 696,
          "s": 847,
          "w": 284,
          "h": 275
        }
      }
    ]
  },
  "metadados": {
    "largura": 2000,
    "altura": 2999
  }
}
