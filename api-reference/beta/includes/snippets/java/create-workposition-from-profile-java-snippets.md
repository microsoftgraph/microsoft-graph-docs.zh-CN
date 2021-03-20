---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: be49d99477d0bba44a8fbb82c12eb740d6e83746
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50974234"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkPosition workPosition = new WorkPosition();
PositionDetail detail = new PositionDetail();
CompanyDetail company = new CompanyDetail();
company.displayName = "Adventureworks Ltd.";
company.department = "Consulting";
company.officeLocation = "AW23/344";
PhysicalAddress address = new PhysicalAddress();
address.type = PhysicalAddressType.BUSINESS;
address.street = "123 Patriachy Ponds";
address.city = "Moscow";
address.countryOrRegion = "Russian Federation";
address.postalCode = "RU-34621";
company.address = address;
company.webUrl = "https://www.adventureworks.com";
detail.company = company;
detail.jobTitle = "Senior Product Branding Manager II";
detail.role = "consulting";
workPosition.detail = detail;
workPosition.isCurrent = true;

graphClient.me().profile().positions()
    .buildRequest()
    .post(workPosition);

```