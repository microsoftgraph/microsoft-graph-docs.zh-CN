---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2adb5c54ae1d29ef8e0450ca2ec2ede390fca4f8
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50967506"
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