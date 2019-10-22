---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f3f66e72ab23f97265a7f15d00d4e206be25a345
ms.sourcegitcommit: d8a425766aa6a56027b8576bbec6a9d1ae3e079c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/21/2019
ms.locfileid: "37553952"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EducationSchool educationSchool = new EducationSchool();
educationSchool.displayName = "Fabrikam High School";
educationSchool.description = "Magnate school for the arts. Los Angeles School District";
educationSchool.status = "String";
educationSchool.externalSource = EducationExternalSource.SIS;
educationSchool.principalEmail = "AmyR@fabrikam.com";
educationSchool.principalName = "Amy Roebuck";
educationSchool.externalPrincipalId = "14007";
educationSchool.highestGrade = "12";
educationSchool.lowestGrade = "9";
educationSchool.schoolNumber = "10002";
PhysicalAddress address = new PhysicalAddress();
address.city = "Los Angeles";
address.countryOrRegion = "United States";
address.postalCode = "98055";
address.state = "CA";
address.street = "12345 Main St.";
educationSchool.address = address;
educationSchool.externalId = "10002";
educationSchool.phone = "+1 (253) 555-0102";

graphClient.education().schools()
    .buildRequest()
    .post(educationSchool);

```