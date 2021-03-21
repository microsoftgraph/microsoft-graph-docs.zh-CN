---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fe0f10ccbe8e72fc6ec3b15a4736735fcdf4419b
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50983394"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkbookCommentReply workbookCommentReply = new WorkbookCommentReply();
workbookCommentReply.content = "This is my reply to the comment.";
workbookCommentReply.contentType = "plain";

graphClient.drive().items("{id}").workbook().comments("{id}").replies()
    .buildRequest()
    .post(workbookCommentReply);

```