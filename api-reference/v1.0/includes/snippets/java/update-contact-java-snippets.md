---
description: 自动生成的文件。 不修改
ms.openlocfilehash: fad9a406cfbeae88af68a6c215d7738c1762e8a3
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35884029"
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
contact.birthday = "1974-07-22";

graphClient.me().contacts("{id}")
    .buildRequest()
    .patch(contact);

```