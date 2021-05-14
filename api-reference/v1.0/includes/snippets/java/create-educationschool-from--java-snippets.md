---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fa6b0bb1d7d5b8cb5e5cd32eb4007ab8f6c4e000
ms.sourcegitcommit: b8b0e88b3ba9a434dc45f5ab640cb46f66fae299
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/13/2021
ms.locfileid: "52474830"
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