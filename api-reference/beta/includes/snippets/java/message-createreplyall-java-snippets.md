---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 16130bb01a2d85498e6664906f4d7db474b05249125d5d837bf055e24df944b2
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57220638"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

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
    .createReplyAll(MessageCreateReplyAllParameterSet
        .newBuilder()
        .withMessage(message)
        .withComment(comment)
        .build())
    .buildRequest()
    .post();

```