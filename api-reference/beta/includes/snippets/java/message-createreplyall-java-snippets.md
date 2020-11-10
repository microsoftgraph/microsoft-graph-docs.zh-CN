---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1373014f644428f326b3f249bab10653c3b3fb3e
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48981567"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Message message = new Message();
LinkedList<Attachment> attachmentsList = new LinkedList<Attachment>();
FileAttachment attachments = new FileAttachment();
attachments.name = "guidelines.txt";
attachments.contentBytes = Base64.getDecoder().decode("bWFjIGFuZCBjaGVlc2UgdG9kYXk=");
attachmentsList.add(attachments);
AttachmentCollectionResponse attachmentCollectionResponse = new AttachmentCollectionResponse();
attachmentCollectionResponse.value = attachmentsList;
AttachmentCollectionPage attachmentCollectionPage = new AttachmentCollectionPage(attachmentCollectionResponse, null);
message.attachments = attachmentCollectionPage;

String comment = "if the project gets approved, please take a look at the attached guidelines before you decide on the name.";

graphClient.me().messages("AAMkADA1MTAAAH5JaKAAA=")
    .createReplyAll(message,comment)
    .buildRequest()
    .post();

```