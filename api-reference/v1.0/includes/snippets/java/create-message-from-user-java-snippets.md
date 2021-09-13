---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e4122834e60be9ddb913dd469a87ddf83caf28b040ad0e05dc70d6001e5bad97
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56903471"
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