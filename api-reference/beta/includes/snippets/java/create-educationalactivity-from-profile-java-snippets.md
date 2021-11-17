---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: cfe8b070b2d9a540d6af98b3c18736085371d295bbb19fa023a9c71bb178535f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56903096"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EducationalActivity educationalActivity = new EducationalActivity();
educationalActivity.completionMonthYear = new DateOnly(1900,1,1);
educationalActivity.endMonthYear = new DateOnly(1900,1,1);
InstitutionData institution = new InstitutionData();
institution.description = null;
institution.displayName = "Colorado State University";
PhysicalAddress location = new PhysicalAddress();
location.type = PhysicalAddressType.BUSINESS;
location.postOfficeBox = null;
location.street = "12000 E Prospect Rd";
location.city = "Fort Collins";
location.state = "Colorado";
location.countryOrRegion = "USA";
location.postalCode = "80525";
institution.location = location;
institution.webUrl = "https://www.colostate.edu";
educationalActivity.institution = institution;
EducationalActivityDetail program = new EducationalActivityDetail();
program.abbreviation = "MBA";
program.activities = null;
program.awards = null;
program.description = "Master of Business Administration with a major in Entreprenuership and Finance.";
program.displayName = "Master of Business Administration";
program.fieldsOfStudy = null;
program.grade = "3.9";
program.notes = null;
program.webUrl = "https://biz.colostate.edu";
educationalActivity.program = program;
educationalActivity.startMonthYear = new DateOnly(1900,1,1);

graphClient.me().profile().educationalActivities()
    .buildRequest()
    .post(educationalActivity);

```