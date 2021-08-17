---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 02503ec9da856609af8ebeb681ee90ba56324ba8ecc7bfe9e9f4dceed3392311
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57279192"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EducationAssignment educationAssignment = new EducationAssignment();
educationAssignment.dueDateTime = OffsetDateTimeSerializer.deserialize("2014-02-01T00:00:00Z");
educationAssignment.displayName = "Midterm 1";
EducationItemBody instructions = new EducationItemBody();
instructions.contentType = BodyType.TEXT;
instructions.content = "Read chapters 1 through 3";
educationAssignment.instructions = instructions;
EducationAssignmentPointsGradeType grading = new EducationAssignmentPointsGradeType();
grading.maxPoints = 100;
educationAssignment.grading = grading;
EducationAssignmentClassRecipient assignTo = new EducationAssignmentClassRecipient();
educationAssignment.assignTo = assignTo;
educationAssignment.status = EducationAssignmentStatus.DRAFT;
educationAssignment.allowStudentsToAddResourcesToSubmission = true;

graphClient.education().classes("8ddcac47-0b45-4cdb-b10a-d36a07a3dd62").assignments()
    .buildRequest()
    .post(educationAssignment);

```