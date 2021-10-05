---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9f3dad5d5983ed32af25deadd415b7d5d21fb34184c5b0dd429c386cadc07260
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57215762"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Message message = new Message();
message.subject = "Party planning";
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

graphClient.me().messages()
    .buildRequest()
    .post(message);

```