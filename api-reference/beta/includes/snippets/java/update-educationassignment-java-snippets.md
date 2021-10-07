---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 98f9f037d0f3fb8294018569828fdee1620def288d8076c785428d8e510413b9
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57161562"
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