---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fb3a42a5bbaab0989bb5e748c9508f1e835384c7
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48980036"
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
MentionCollectionResponse mentionCollectionResponse = new MentionCollectionResponse();
mentionCollectionResponse.value = mentionsList;
MentionCollectionPage mentionCollectionPage = new MentionCollectionPage(mentionCollectionResponse, null);
message.mentions = mentionCollectionPage;

graphClient.me()
    .sendMail(message,null)
    .buildRequest()
    .post();

```