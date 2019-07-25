---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 876729ef5f09c2b2e552f268786974798d3010ec
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35887782"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EducationUser educationUser = new EducationUser();
educationUser.displayName = "Dion Matheson";
educationUser.givenName = "Dion";
educationUser.middleName = null;
educationUser.surname = "Matheson";
educationUser.mail = "DionM@contoso.com";
educationUser.mobilePhone = "+1 (253) 555-0101";
IdentitySet createdBy = new IdentitySet();
Identity user = new Identity();
user.displayName = "Susana Rocha";
user.id = "14012";
createdBy.user = user;
educationUser.createdBy = createdBy;
educationUser.externalSource = EducationExternalSource.SIS;
PhysicalAddress mailingAddress = new PhysicalAddress();
mailingAddress.city = "Los Angeles";
mailingAddress.countryOrRegion = "United States";
mailingAddress.postalCode = "98055";
mailingAddress.state = "CA";
mailingAddress.street = "12345 Main St.";
educationUser.mailingAddress = mailingAddress;
educationUser.primaryRole = EducationUserRole.STUDENT;
PhysicalAddress residenceAddress = new PhysicalAddress();
residenceAddress.city = "Los Angeles";
residenceAddress.countryOrRegion = "United States";
residenceAddress.postalCode = "98055";
residenceAddress.state = "CA";
residenceAddress.street = "12345 Main St.";
educationUser.residenceAddress = residenceAddress;

graphClient.education().users()
    .buildRequest()
    .post(educationUser);

```