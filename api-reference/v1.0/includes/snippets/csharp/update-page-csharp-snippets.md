---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 56538c864a7444524972f08534dba1eb538d10172303d644da0773b6cdf818d1
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57333923"
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