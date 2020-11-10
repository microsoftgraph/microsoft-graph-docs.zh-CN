---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a4f965aec87e095f83bd0f5c6cf14b648e0ab991
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48972939"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

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