---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d3a80513a04c153a900812398bf0507ae27b9cf4
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48966487"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EducationAssignment educationAssignment = new EducationAssignment();
educationAssignment.displayName = "Week 1 reading assignment";
EducationItemBody instructions = new EducationItemBody();
instructions.contentType = BodyType.TEXT;
instructions.content = "Read chapters 1 through 3";
educationAssignment.instructions = instructions;
educationAssignment.dueDateTime = CalendarSerializer.deserialize("2014-02-01T00:00:00Z");

graphClient.education().classes("11021").assignments("19002")
    .buildRequest()
    .patch(educationAssignment);

```