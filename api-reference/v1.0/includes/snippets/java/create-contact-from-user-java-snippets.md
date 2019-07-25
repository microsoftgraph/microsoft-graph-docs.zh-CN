---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b36861e09dbc769fd34f2d4630787774f62201ea
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35885674"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Contact contact = new Contact();
contact.givenName = "Pavel";
contact.surname = "Bansky";
LinkedList<EmailAddress> emailAddressesList = new LinkedList<EmailAddress>();
EmailAddress emailAddresses = new EmailAddress();
emailAddresses.address = "pavelb@fabrikam.onmicrosoft.com";
emailAddresses.name = "Pavel Bansky";
emailAddressesList.add(emailAddresses);
contact.emailAddresses = emailAddressesList;
LinkedList<String> businessPhonesList = new LinkedList<String>();
businessPhonesList.add("+1 732 555 0102");
contact.businessPhones = businessPhonesList;

graphClient.me().contacts()
    .buildRequest()
    .post(contact);

```