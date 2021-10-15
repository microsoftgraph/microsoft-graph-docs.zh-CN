---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 20f98d8080c00be94356c19c01675c9ceef63f7b
ms.sourcegitcommit: 8ae180a32dbd5a2b12512aee64699a2c23b8678b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/14/2021
ms.locfileid: "60365837"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EducationAssignment educationAssignment = new EducationAssignment();
educationAssignment.displayName = "Reading and review test 09.03 #5";
EducationItemBody instructions = new EducationItemBody();
instructions.contentType = BodyType.TEXT;
instructions.content = "Read chapter 5 and write your review";
educationAssignment.instructions = instructions;
educationAssignment.dueDateTime = OffsetDateTimeSerializer.deserialize("2021-09-10T00:00:00Z");
educationAssignment.addedStudentAction = EducationAddedStudentAction.NONE;
educationAssignment.addToCalendarAction = EducationAddToCalendarOptions.STUDENTS_AND_PUBLISHER;

graphClient.education().classes("72a7baec-c3e9-4213-a850-f62de0adad5f").assignments("4679bc1b-90c5-45af-ae1a-d5357672ed39")
    .buildRequest()
    .patch(educationAssignment);

```