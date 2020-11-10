---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fb54ee7e87db7aa12a5e9d5b1a1dd06e196a08be
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48967404"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Message message = new Message();
LinkedList<Recipient> toRecipientsList = new LinkedList<Recipient>();
Recipient toRecipients = new Recipient();
EmailAddress emailAddress = new EmailAddress();
emailAddress.address = "samanthab@contoso.onmicrosoft.com";
emailAddress.name = "Samantha Booth";
toRecipients.emailAddress = emailAddress;
toRecipientsList.add(toRecipients);
Recipient toRecipients1 = new Recipient();
EmailAddress emailAddress1 = new EmailAddress();
emailAddress1.address = "randiw@contoso.onmicrosoft.com";
emailAddress1.name = "Randi Welch";
toRecipients1.emailAddress = emailAddress1;
toRecipientsList.add(toRecipients1);
message.toRecipients = toRecipientsList;

String comment = "Samantha, Randi, would you name the group please?";

graphClient.me().messages("AAMkADA1MTAAAAqldOAAA=")
    .reply(message,comment)
    .buildRequest()
    .post();

```