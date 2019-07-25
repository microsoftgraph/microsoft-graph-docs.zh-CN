---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 969ab8d39315ec631df3f102207189d73e67144c
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35879626"
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
    .forward(message,comment,toRecipientsList)
    .buildRequest()
    .post();

```