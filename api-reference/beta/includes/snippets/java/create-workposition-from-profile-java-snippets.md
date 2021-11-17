---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d77d505e9b65a17bc8ce93f6a84a91e70d03c2ff27f18bc99871971d133765d7
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57161844"
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