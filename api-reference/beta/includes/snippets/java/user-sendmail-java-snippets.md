---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: da9c6374a066e4b042c9879a87bc2fcc7f1f494eac3c0d32305c718fcf15679e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57277730"
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
    .sendMail(UserSendMailParameterSet
        .newBuilder()
        .withMessage(message)
        .withSaveToSentItems(saveToSentItems)
        .build())
    .buildRequest()
    .post();

```