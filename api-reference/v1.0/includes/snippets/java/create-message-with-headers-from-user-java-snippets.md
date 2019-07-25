---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 09e3cba25597aed7dab832ba0cf047753060061a
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35885640"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Message message = new Message();
message.subject = "9/8/2018: concert";
ItemBody body = new ItemBody();
body.contentType = BodyType.HTML;
body.content = "The group represents Washington.";
message.body = body;
LinkedList<Recipient> toRecipientsList = new LinkedList<Recipient>();
Recipient toRecipients = new Recipient();
EmailAddress emailAddress = new EmailAddress();
emailAddress.address = "AlexW@contoso.OnMicrosoft.com";
toRecipients.emailAddress = emailAddress;
toRecipientsList.add(toRecipients);
message.toRecipients = toRecipientsList;
LinkedList<InternetMessageHeader> internetMessageHeadersList = new LinkedList<InternetMessageHeader>();
InternetMessageHeader internetMessageHeaders = new InternetMessageHeader();
internetMessageHeaders.name = "x-custom-header-group-name";
internetMessageHeaders.value = "Washington";
internetMessageHeadersList.add(internetMessageHeaders);
InternetMessageHeader internetMessageHeaders1 = new InternetMessageHeader();
internetMessageHeaders1.name = "x-custom-header-group-id";
internetMessageHeaders1.value = "WA001";
internetMessageHeadersList.add(internetMessageHeaders1);
message.internetMessageHeaders = internetMessageHeadersList;

graphClient.me().messages()
    .buildRequest()
    .post(message);

```