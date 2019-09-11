---
description: 自动生成的文件。 不修改
ms.openlocfilehash: bf3197feeb8e054ee1ec8c20ce4a17cf8ce4d4cf
ms.sourcegitcommit: d8a58221ed1f2b7b7073fd621da4737e11ba53c5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/11/2019
ms.locfileid: "36839073"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkbookCommentReply workbookCommentReply = new WorkbookCommentReply();
workbookCommentReply.content = "This is my reply to the comment.";
workbookCommentReply.contentType = "plain";

graphClient.drive().root().workbook().comments("{id}").replies()
    .buildRequest()
    .post(workbookCommentReply);

```