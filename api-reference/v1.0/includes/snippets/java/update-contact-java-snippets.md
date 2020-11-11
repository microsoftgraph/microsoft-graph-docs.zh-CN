---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8eb0895985b5fcaae38b2c7aea4462ef96f33bf0
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48982895"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Contact contact = new Contact();
PhysicalAddress homeAddress = new PhysicalAddress();
homeAddress.street = "123 Some street";
homeAddress.city = "Seattle";
homeAddress.state = "WA";
homeAddress.postalCode = "98121";
contact.homeAddress = homeAddress;
contact.birthday = CalendarSerializer.deserialize("1974-07-22");

graphClient.me().contacts("{id}")
    .buildRequest()
    .patch(contact);

```