---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: db779d9441f5bba17e015c29a2175614b9e128b7
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48957152"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Contact contact = new Contact();
LinkedList<TypedEmailAddress> emailAddressesList = new LinkedList<TypedEmailAddress>();
TypedEmailAddress emailAddresses = new TypedEmailAddress();
emailAddresses.type = EmailType.PERSONAL;
emailAddresses.name = "Pavel Bansky";
emailAddresses.address = "pavelb@adatum.onmicrosoft.com";
emailAddressesList.add(emailAddresses);
TypedEmailAddress emailAddresses1 = new TypedEmailAddress();
emailAddresses1.address = "pavelb@fabrikam.onmicrosoft.com";
emailAddresses1.name = "Pavel Bansky";
emailAddresses1.type = EmailType.OTHER;
emailAddresses1.otherLabel = "Volunteer work";
emailAddressesList.add(emailAddresses1);
contact.emailAddresses = emailAddressesList;

graphClient.me().contacts("AAMkADh6v5AAAvgTCEAAA=")
    .buildRequest()
    .patch(contact);

```