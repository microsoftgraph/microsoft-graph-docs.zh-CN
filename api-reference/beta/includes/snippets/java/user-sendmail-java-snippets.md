---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 3b3b1702d4d02933f249d1d362ac02d64bf5cdfd
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35866705"
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