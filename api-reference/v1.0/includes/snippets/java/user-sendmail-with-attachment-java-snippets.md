---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ce583d07a39ec9c4badf8ed07b8eb13bb9512685
ms.sourcegitcommit: 7b286637aa332cfd534a41526950b4f6272e0fd7
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/05/2020
ms.locfileid: "41774349"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

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
attachments.contentBytes = "SGVsbG8gV29ybGQh";
attachmentsList.add(attachments);
message.attachments = attachmentsList;

graphClient.me()
    .sendMail(message,null)
    .buildRequest()
    .post();

```