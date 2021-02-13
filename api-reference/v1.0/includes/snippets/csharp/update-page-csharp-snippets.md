---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 95dc939f74e35fe5e5522c18dd11135f644eae05
ms.sourcegitcommit: 48fff935d56fe96e97577a80a3a0aa15c45419ba
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/10/2021
ms.locfileid: "50179158"
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

await graphClient.Me.Onenote.Pages["{id}"]
    .Request()
    .UpdateAsync(pages);

```