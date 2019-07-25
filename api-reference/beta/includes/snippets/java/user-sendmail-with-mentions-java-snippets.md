---
description: 自动生成的文件。 不修改
ms.openlocfilehash: f57a749a6b2ffa5371e30b885f02ec1f5795813f
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35866707"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Message message = new Message();
message.subject = "Project kickoff";
LinkedList<Recipient> toRecipientsList = new LinkedList<Recipient>();
Recipient toRecipients = new Recipient();
EmailAddress emailAddress = new EmailAddress();
emailAddress.name = "Samantha Booth";
emailAddress.address = "samanthab@contoso.onmicrosoft.com";
toRecipients.emailAddress = emailAddress;
toRecipientsList.add(toRecipients);
message.toRecipients = toRecipientsList;
LinkedList<Mention> mentionsList = new LinkedList<Mention>();
Mention mentions = new Mention();
EmailAddress mentioned = new EmailAddress();
mentioned.name = "Dana Swope";
mentioned.address = "danas@contoso.onmicrosoft.com";
mentions.mentioned = mentioned;
mentionsList.add(mentions);
message.mentions = mentionsList;

graphClient.me()
    .sendMail(message,saveToSentItems)
    .buildRequest()
    .post();

```