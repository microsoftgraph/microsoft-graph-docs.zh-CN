---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fa7dc6d74c8231bef5171bd48237708a89370965ca667fd552873d0edd4513e3
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57164325"
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