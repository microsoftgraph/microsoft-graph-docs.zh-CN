---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2dd1209b68eda85d7883994cde4c1805802de056
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50971958"
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