---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bd74551a2e3fc045435016e6213f33cef8b8b020
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50976280"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

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