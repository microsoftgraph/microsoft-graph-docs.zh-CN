---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8ff920f5555f4b13cb303e1f3c9be53302ea089a
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48966642"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

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