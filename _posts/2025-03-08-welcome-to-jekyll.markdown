---
layout: post
title:  "Welcome to Jekyll!"
date:   2025-03-08 22:19:02 -0300
categories: jekyll update
---
# Como Criar uma Extensão para o Revit Usando pyRevit e Dynamo 🚀

Automatizar tarefas no Autodesk Revit pode economizar horas de trabalho e reduzir erros. Com o **Dynamo** e o **pyRevit**, podemos criar ferramentas personalizadas para otimizar fluxos de trabalho e facilitar processos repetitivos.

## Introdução  
O **Dynamo** é uma ferramenta de automação visual baseada em **nós**, permitindo criar scripts para tarefas repetitivas no Revit.  
O **pyRevit** é uma extensão poderosa para personalizar o Revit, permitindo que desenvolvedores criem seus próprios plugins e ferramentas.

## Motivação  
Por que criar uma extensão personalizada?  
> ✅ Organiza melhor seus scripts Dynamo e Python  
> ✅ Facilita a execução dentro do Revit com um clique  
> ✅ Permite compartilhar ferramentas com sua equipe  
> ✅ Aumenta a produtividade e reduz retrabalho

## Passo a Passo  

### 🔹 Criando a Estrutura da Extensão no pyRevit  
1. Acesse a pasta de extensões do pyRevit (`%AppData%\pyRevit\Extensions\` no Windows).  
2. Crie uma pasta com o nome da sua extensão (exemplo: `MinhaExtensao.extension`).  
3. Dentro dela, crie uma subpasta chamada `MinhaAba.tab` e outra `MeuPainel.panel`.  
4. Adicione um script dentro da pasta `MeuPainel.panel` (exemplo: `MeuScript.pushbutton`).  

### 🔹 Como Adicionar Scripts do Dynamo  
1. Salve seu arquivo **Dynamo (.dyn)** em um local acessível.  
2. No pyRevit, crie um **arquivo `.script`** dentro da pasta do botão.  
3. Edite o `.script` para executar o Dynamo automaticamente:

```python
import subprocess  
dynamo_file = r"C:\Caminho\Para\SeuScript.dyn"  
subprocess.Popen(["C:\\Program Files\\Dynamo\\DynamoSandbox.exe", dynamo_file])
```

Isso fará com que seu script Dynamo rode direto pelo botão no pyRevit! 🎯

## Exemplos de Aplicações Práticas
Aqui estão algumas ideias de automação que você pode implementar:
  > ✔ Criar um botão para renomear múltiplas famílias no Revit 
  > ✔ Gerar folhas e vistas automaticamente 
  > ✔ Atualizar parâmetros de elementos 
  > ✔ Exportar dados para Excel diretamente do Revit 