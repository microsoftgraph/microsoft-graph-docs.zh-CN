---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 02ab654e0c1f3624d7c8afab3087e5fdedae1f150fd5c34404602747236d4119
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57104663"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Contact contact = new Contact();
contact.givenName = "Pavel";
contact.surname = "Bansky";
LinkedList<TypedEmailAddress> emailAddressesList = new LinkedList<TypedEmailAddress>();
TypedEmailAddress emailAddresses = new TypedEmailAddress();
emailAddresses.address = "pavelb@contoso.onmicrosoft.com";
emailAddresses.name = "Pavel Bansky";
emailAddresses.type = EmailType.PERSONAL;
emailAddressesList.add(emailAddresses);
TypedEmailAddress emailAddresses1 = new TypedEmailAddress();
emailAddresses1.address = "pavelb@fabrikam.onmicrosoft.com";
emailAddresses1.name = "Pavel Bansky";
emailAddresses1.type = EmailType.OTHER;
emailAddresses1.otherLabel = "Volunteer work";
emailAddressesList.add(emailAddresses1);
contact.emailAddresses = emailAddressesList;
LinkedList<Phone> phonesList = new LinkedList<Phone>();
Phone phones = new Phone();
phones.number = "+1 732 555 0102";
phones.type = PhoneType.BUSINESS;
phonesList.add(phones);
contact.phones = phonesList;

graphClient.me().contacts()
    .buildRequest()
    .post(contact);

```