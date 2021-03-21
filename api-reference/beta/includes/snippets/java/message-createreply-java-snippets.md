---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 447d373aedf4b933ca09f02fdb4683a944e56d99
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50970194"
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