---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7d0c48656b447b79810e6a31a12a872697187e0f
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50796291"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var stream = new System.IO.MemoryStream(Encoding.UTF8.GetBytes(@"[
   {
    'target':'#para-id',
    'action':'insert',
    'position':'before',
    'content':'<img src=""image-url-or-part-name"" alt=""image-alt-text"" />'
  }, 
  {
    'target':'#list-id',
    'action':'append',
    'content':'<li>new-page-content</li>'
  }
]
"));

var pages = new OnenotePage();
pages.Content = stream;

await graphClient.Me.Onenote.Pages["{onenotePage-id}"]
    .Request()
    .UpdateAsync(pages);

```