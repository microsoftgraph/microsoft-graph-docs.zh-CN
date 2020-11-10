---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 09e3cba25597aed7dab832ba0cf047753060061a
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48977061"
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