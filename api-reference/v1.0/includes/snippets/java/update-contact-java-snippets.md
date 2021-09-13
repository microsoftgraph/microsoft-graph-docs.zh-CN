---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b134a4f259708ad7172be9a798b50111a7a8b49a0ed61c12ce33a038afbb4c74
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57161626"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Contact contact = new Contact();
PhysicalAddress homeAddress = new PhysicalAddress();
homeAddress.street = "123 Some street";
homeAddress.city = "Seattle";
homeAddress.state = "WA";
homeAddress.postalCode = "98121";
contact.homeAddress = homeAddress;
contact.birthday = OffsetDateTimeSerializer.deserialize("1974-07-22");

graphClient.me().contacts("{id}")
    .buildRequest()
    .patch(contact);

```