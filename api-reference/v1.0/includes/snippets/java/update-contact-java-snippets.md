---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: eaf55cacf4b6b652dd7cfcadb9dc5afce5ad4fcc
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50978247"
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