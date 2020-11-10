---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0c771d4db7afe6b900052a0f24595ca2a28ac084
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48974631"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

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