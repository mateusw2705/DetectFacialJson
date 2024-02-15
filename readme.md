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
!(azure/pessoa.png)
!(images/pessoa.jpg)

## Passo 3: Interpretar o JSON Retornado

O JSON retornado conterá informações sobre a detecção de objetos na imagem. Aqui está um exemplo de como o JSON pode ser estruturado:

```json
{
  "objects": [
    {
      "label": "car",
      "confidence": 0.85,
      "bounding_box": {
        "x": 100,
        "y": 150,
        "width": 200,
        "height": 100
      }
    },
    {
      "label": "person",
      "confidence": 0.75,
      "bounding_box": {
        "x": 50,
        "y": 75,
        "width": 150,
        "height": 300
      }
    }
  ]
}
