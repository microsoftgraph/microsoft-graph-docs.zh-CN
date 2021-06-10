---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0374d37c9ad499f37672d2bd89eefcc1510bb142
ms.sourcegitcommit: 503c72036c376a30e08c29df8e7730a7afcab66e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/10/2021
ms.locfileid: "52871549"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EducationAssignment educationAssignment = new EducationAssignment();
educationAssignment.displayName = "Week 1 reading assignment";
EducationItemBody instructions = new EducationItemBody();
instructions.contentType = BodyType.TEXT;
instructions.content = "Read chapters 1 through 3";
educationAssignment.instructions = instructions;
educationAssignment.dueDateTime = OffsetDateTimeSerializer.deserialize("2014-02-01T00:00:00Z");
educationAssignment.addedStudentAction = EducationAddedStudentAction.NONE;
educationAssignment.addToCalendarAction = EducationAddToCalendarOptions.STUDENTS_AND_PUBLISHER;

graphClient.education().classes("11021").assignments("19002")
    .buildRequest()
    .patch(educationAssignment);

```