---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: db598cdd63c4252957dc9b941bbe29efb50872a4
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50975936"
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

String comment = "Dana, just want to make sure you get this.";

graphClient.me().messages("AAMkADA1MTAAAH5JaLAAA=")
    .forward(MessageForwardParameterSet
        .newBuilder()
        .withToRecipients(null)
        .withMessage(message)
        .withComment(comment)
        .build())
    .buildRequest()
    .post();

```