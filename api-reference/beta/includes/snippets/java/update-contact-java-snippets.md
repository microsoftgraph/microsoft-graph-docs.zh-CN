---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 88083cf70ecd113a23379f81d9b41041e1492a7bf73320529cc3b7dd819fd300
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57329060"
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