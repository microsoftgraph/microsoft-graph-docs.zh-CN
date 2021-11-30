---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2dd1209b68eda85d7883994cde4c1805802de056
ms.sourcegitcommit: e497ed9bb56400bdd2bb53d52ddf057d9966220b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/30/2021
ms.locfileid: "61226871"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

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