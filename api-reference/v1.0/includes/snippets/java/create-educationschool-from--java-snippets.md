---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ebbde6775c845f674e217915ac1b2ac1eb08a451f0fd79fc2cf34bfaeb84283c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56902279"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EducationSchool educationSchool = new EducationSchool();
educationSchool.displayName = "String";
educationSchool.description = "String";
educationSchool.externalSource = EducationExternalSource.SIS;
educationSchool.externalSourceDetail = "String";
educationSchool.principalEmail = "String";
educationSchool.principalName = "String";
educationSchool.externalPrincipalId = "String";
educationSchool.lowestGrade = "String";
educationSchool.highestGrade = "String";
educationSchool.schoolNumber = "String";
educationSchool.externalId = "String";
educationSchool.phone = "String";
educationSchool.fax = "String";
IdentitySet createdBy = new IdentitySet();
educationSchool.createdBy = createdBy;
PhysicalAddress address = new PhysicalAddress();
educationSchool.address = address;

graphClient.education().schools()
    .buildRequest()
    .post(educationSchool);

```