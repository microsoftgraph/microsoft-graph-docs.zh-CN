---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 59129f8000c3fac3847a90d6cead672990167e3ff85e50d3a3df98c72a5347a6
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57161966"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Message message = new Message();
message.subject = "Meet for lunch?";
ItemBody body = new ItemBody();
body.contentType = BodyType.TEXT;
body.content = "The new cafeteria is open.";
message.body = body;
LinkedList<Recipient> toRecipientsList = new LinkedList<Recipient>();
Recipient toRecipients = new Recipient();
EmailAddress emailAddress = new EmailAddress();
emailAddress.address = "meganb@contoso.onmicrosoft.com";
toRecipients.emailAddress = emailAddress;
toRecipientsList.add(toRecipients);
message.toRecipients = toRecipientsList;
LinkedList<Attachment> attachmentsList = new LinkedList<Attachment>();
FileAttachment attachments = new FileAttachment();
attachments.name = "attachment.txt";
attachments.contentType = "text/plain";
attachments.contentBytes = Base64.getDecoder().decode("SGVsbG8gV29ybGQh");
attachmentsList.add(attachments);
AttachmentCollectionResponse attachmentCollectionResponse = new AttachmentCollectionResponse();
attachmentCollectionResponse.value = attachmentsList;
AttachmentCollectionPage attachmentCollectionPage = new AttachmentCollectionPage(attachmentCollectionResponse, null);
message.attachments = attachmentCollectionPage;

graphClient.me()
    .sendMail(UserSendMailParameterSet
        .newBuilder()
        .withMessage(message)
        .withSaveToSentItems(null)
        .build())
    .buildRequest()
    .post();

```