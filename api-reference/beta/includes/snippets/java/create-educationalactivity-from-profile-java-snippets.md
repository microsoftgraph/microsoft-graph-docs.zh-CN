---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b1e79aef461fdfbb6f500f2b33b14a741f6553af
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50977575"
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