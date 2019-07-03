---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 5bf168a4f16b9c3bf06af4699d03846ab8659366
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35493046"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var Stream = new List<Stream>()
{
    new Stream
    {
        Target = "#para-id",
        Action = "insert",
        Position = "before",
        Content = "<img src=\"image-url-or-part-name\" alt=\"image-alt-text\" />"
    },
    new Stream
    {
        Target = "#list-id",
        Action = "append",
        Content = "<li>new-page-content</li>"
    }
};

var pages = new OnenotePage();
pages.Content = content;

await graphClient.Me.Onenote.Pages["{id}"]
    .Request()
    .UpdateAsync(pages);

```