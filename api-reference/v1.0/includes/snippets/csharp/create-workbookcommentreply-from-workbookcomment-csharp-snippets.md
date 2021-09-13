---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9cb28de721e33fb9bc1f0a1f6ba7d440bbb4968611a4383029ce26a87dba0434
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57328830"
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