---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3b3b1702d4d02933f249d1d362ac02d64bf5cdfd
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48980037"
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
emailAddress.address = "samanthab@contoso.onmicrosoft.com";
toRecipients.emailAddress = emailAddress;
toRecipientsList.add(toRecipients);
message.toRecipients = toRecipientsList;
LinkedList<Recipient> ccRecipientsList = new LinkedList<Recipient>();
Recipient ccRecipients = new Recipient();
EmailAddress emailAddress1 = new EmailAddress();
emailAddress1.address = "danas@contoso.onmicrosoft.com";
ccRecipients.emailAddress = emailAddress1;
ccRecipientsList.add(ccRecipients);
message.ccRecipients = ccRecipientsList;

boolean saveToSentItems = false;

graphClient.me()
    .sendMail(message,saveToSentItems)
    .buildRequest()
    .post();

```