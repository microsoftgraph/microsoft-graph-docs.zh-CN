---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 82870b6c340eef55ed5c8bb28b2a27ac958dbbac
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35879733"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Message message = new Message();
LinkedList<Attachment> attachmentsList = new LinkedList<Attachment>();
Attachment attachments = new Attachment();
attachments.additionalDataManager().put("@odata.type", new JsonPrimitive("#microsoft.graph.fileAttachment"));
attachments.name = "guidelines.txt";
attachments.contentBytes = "bWFjIGFuZCBjaGVlc2UgdG9kYXk=";
attachmentsList.add(attachments);
message.attachments = attachmentsList;

String comment = "if the project gets approved, please take a look at the attached guidelines before you decide on the name.";

graphClient.me().messages("AAMkADA1MTAAAH5JaKAAA=")
    .createReplyAll(message,comment)
    .buildRequest()
    .post();

```