---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: df1fad31fec4616a3173c6e688e3eaa37fad331c
ms.sourcegitcommit: 2f78ac96a9b0462626a242429055ef824590bd3f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2020
ms.locfileid: "41495836"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookCommentReply = new WorkbookCommentReply
{
    Content = "This is my reply to the comment.",
    ContentType = "plain"
};

await graphClient.Drive.Items["{id}"].Workbook.Comments["{id}"].Replies
    .Request()
    .AddAsync(workbookCommentReply);

```