---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 78d0a468408860559f397b5bffbad86c95adaeba
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35878351"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Message message = new Message();
message.subject = "Annual review";
ItemBody body = new ItemBody();
body.contentType = BodyType.HTML;
body.content = "You should be proud!";
message.body = body;
LinkedList<Recipient> toRecipientsList = new LinkedList<Recipient>();
Recipient toRecipients = new Recipient();
EmailAddress emailAddress = new EmailAddress();
emailAddress.address = "rufus@contoso.com";
toRecipients.emailAddress = emailAddress;
toRecipientsList.add(toRecipients);
message.toRecipients = toRecipientsList;
LinkedList<Extension> extensionsList = new LinkedList<Extension>();
Extension extensions = new Extension();
extensions.additionalDataManager().put("@odata.type", new JsonPrimitive("microsoft.graph.openTypeExtension"));
extensions.extensionName = "Com.Contoso.Referral";
extensions.companyName = "Wingtip Toys";
extensions.expirationDate = "2015-12-30T11:00:00Z";
extensions.dealValue = 10000;
extensionsList.add(extensions);
message.extensions = extensionsList;

graphClient.me().messages()
    .buildRequest()
    .post(message);

```