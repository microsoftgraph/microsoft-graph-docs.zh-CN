---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 26abdbae29a56b37a196b7101160ecf3b0b1aaa8
ms.sourcegitcommit: 7a6231aeb570ff45d01b3db3df07a411f9f60fd1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/27/2020
ms.locfileid: "44384338"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EducationSchool educationSchool = new EducationSchool();
educationSchool.displayName = "Fabrikam High School";
educationSchool.description = "Magnate school for the arts. Los Angeles School District";
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