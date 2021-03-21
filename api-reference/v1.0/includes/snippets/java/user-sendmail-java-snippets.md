---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 43d99ef3a7d5e6d8d73741ebf2a70c014a777fa8
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50971499"
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
emailAddress.address = "fannyd@contoso.onmicrosoft.com";
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
    .sendMail(UserSendMailParameterSet
        .newBuilder()
        .withMessage(message)
        .withSaveToSentItems(saveToSentItems)
        .build())
    .buildRequest()
    .post();

```