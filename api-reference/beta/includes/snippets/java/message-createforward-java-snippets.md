---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4f09892fd376b3298a48904600dbbd1dc9f63c06cd0a8c1adb75a461587d9e09
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57104774"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Message message = new Message();
message.isDeliveryReceiptRequested = true;
LinkedList<Recipient> toRecipientsList = new LinkedList<Recipient>();
Recipient toRecipients = new Recipient();
EmailAddress emailAddress = new EmailAddress();
emailAddress.address = "danas@contoso.onmicrosoft.com";
emailAddress.name = "Dana Swope";
toRecipients.emailAddress = emailAddress;
toRecipientsList.add(toRecipients);
message.toRecipients = toRecipientsList;

String comment = "Dana, just want to make sure you get this; you'll need this if the project gets approved.";

graphClient.me().messages("AAMkADA1MTAAAH5JaLAAA=")
    .createForward(MessageCreateForwardParameterSet
        .newBuilder()
        .withToRecipients(null)
        .withMessage(message)
        .withComment(comment)
        .build())
    .buildRequest()
    .post();

```