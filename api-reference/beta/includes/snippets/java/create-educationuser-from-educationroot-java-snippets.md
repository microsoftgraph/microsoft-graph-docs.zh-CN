---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d1180277ad8377a17917600d53086e7cbff63b4a16ecb66d9747835445f2a25d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57105778"
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