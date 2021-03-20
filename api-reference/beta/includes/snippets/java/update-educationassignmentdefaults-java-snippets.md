---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8c5f10523aaaf901ceb10d81f1b7072d84281a3e
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50977280"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EducationAssignmentDefaults educationAssignmentDefaults = new EducationAssignmentDefaults();
educationAssignmentDefaults.addedStudentAction = EducationAddedStudentAction.ASSIGN_IF_OPEN;
educationAssignmentDefaults.notificationChannelUrl = "https://graph.microsoft.com/beta/teams('id')/channels('id')";

graphClient.education().classes("{id}").assignmentDefaults()
    .buildRequest()
    .patch(educationAssignmentDefaults);

```