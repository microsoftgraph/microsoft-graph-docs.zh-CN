---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c19c44690a4ce4f775da58dfffa5d0f2f2cc1bc6
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50804918"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookCommentReply = new WorkbookCommentReply
{
    Content = "This is my reply to the comment.",
    ContentType = "plain"
};

await graphClient.Drive.Items["{driveItem-id}"].Workbook.Comments["{workbookComment-id}"].Replies
    .Request()
    .AddAsync(workbookCommentReply);

```