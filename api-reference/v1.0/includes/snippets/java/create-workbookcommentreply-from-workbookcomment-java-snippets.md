---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7912d99a33748fff5dfa51479b65871a62f10913
ms.sourcegitcommit: 2f78ac96a9b0462626a242429055ef824590bd3f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2020
ms.locfileid: "41496286"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkbookCommentReply workbookCommentReply = new WorkbookCommentReply();
workbookCommentReply.content = "This is my reply to the comment.";
workbookCommentReply.contentType = "plain";

graphClient.drive().items("{id}").workbook().comments("{id}").replies()
    .buildRequest()
    .post(workbookCommentReply);

```