---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3930af239c2b416098e253972cac8640f10caf4c
ms.sourcegitcommit: 503c72036c376a30e08c29df8e7730a7afcab66e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/10/2021
ms.locfileid: "52871601"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EducationAssignmentDefaults educationAssignmentDefaults = new EducationAssignmentDefaults();
educationAssignmentDefaults.addedStudentAction = EducationAddedStudentAction.ASSIGN_IF_OPEN;
educationAssignmentDefaults.addToCalendarAction = EducationAddToCalendarOptions.STUDENTS_AND_TEAM_OWNERS;
educationAssignmentDefaults.notificationChannelUrl = "https://graph.microsoft.com/beta/teams('id')/channels('id')";

graphClient.education().classes("{id}").assignmentDefaults()
    .buildRequest()
    .patch(educationAssignmentDefaults);

```