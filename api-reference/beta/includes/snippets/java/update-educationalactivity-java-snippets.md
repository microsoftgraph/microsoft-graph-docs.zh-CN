---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6abd2dffdf97f2d1d55fcdf9058a2b3f35a188cf
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50983026"
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