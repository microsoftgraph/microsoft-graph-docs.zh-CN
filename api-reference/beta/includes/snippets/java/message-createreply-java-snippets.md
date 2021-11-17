---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fb41e7453082532de65c4a64efc0bd67fdab01c9c819205f9d7ed23b1376c631
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57278064"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

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

String comment = "Samantha, Randi, would you name the group if the project is approved, please?";

graphClient.me().messages("AAMkADA1MTAAAAqldOAAA=")
    .createReply(MessageCreateReplyParameterSet
        .newBuilder()
        .withMessage(message)
        .withComment(comment)
        .build())
    .buildRequest()
    .post();

```