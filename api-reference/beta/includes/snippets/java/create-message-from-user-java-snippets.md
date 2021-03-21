---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4ecbf7e1f3c6b6800b2f37af688604fcae80a090
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50978675"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

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