---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2504486aee2ed984f758baf6c977127ce9f9afa567bc1ca23ceb55440dd4c2ff
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57278308"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EducationalActivity educationalActivity = new EducationalActivity();
InstitutionData institution = new InstitutionData();
PhysicalAddress location = new PhysicalAddress();
location.type = PhysicalAddressType.BUSINESS;
location.postOfficeBox = null;
location.street = "12000 E Prospect Rd";
location.city = "Fort Collins";
location.state = "Colorado";
location.countryOrRegion = "USA";
location.postalCode = "80525";
institution.location = location;
educationalActivity.institution = institution;

graphClient.me().profile().educationalActivities("{id}")
    .buildRequest()
    .patch(educationalActivity);

```