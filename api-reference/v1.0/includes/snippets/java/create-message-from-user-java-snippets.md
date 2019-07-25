---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 509764ccd0f2828d09543892c2dc943900cab6fc
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35885641"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Message message = new Message();
message.subject = "Did you see last night's game?";
message.importance = Importance.LOW;
ItemBody body = new ItemBody();
body.contentType = BodyType.HTML;
body.content = "They were <b>awesome</b>!";
message.body = body;
LinkedList<Recipient> toRecipientsList = new LinkedList<Recipient>();
Recipient toRecipients = new Recipient();
EmailAddress emailAddress = new EmailAddress();
emailAddress.address = "AdeleV@contoso.onmicrosoft.com";
toRecipients.emailAddress = emailAddress;
toRecipientsList.add(toRecipients);
message.toRecipients = toRecipientsList;

graphClient.me().messages()
    .buildRequest()
    .post(message);

```