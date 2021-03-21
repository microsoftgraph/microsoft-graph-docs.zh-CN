---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6d9bd81281e9a7bf45b12144af8c43af232a101e
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50974620"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

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