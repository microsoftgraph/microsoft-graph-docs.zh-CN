---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5e9b27792f65d47f8844f2910d38fd18462dcfcc
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48978565"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

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
    .forward(null,message,comment)
    .buildRequest()
    .post();

```