---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b7e83e7382b4c4a8471d2b71563a84ec1914d715
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2021
ms.locfileid: "50470318"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EducationAssignmentDefaults educationAssignmentDefaults = new EducationAssignmentDefaults();
educationAssignmentDefaults.addedStudentAction = EducationAddedStudentAction.ASSIGN_IF_OPEN;
educationAssignmentDefaults.notificationChannelUrl = "https://graph.microsoft.com/beta/teams('id')/channels('id')";

graphClient.education().classes("{id}").assignmentDefaults()
    .buildRequest()
    .patch(educationAssignmentDefaults);

```