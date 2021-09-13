---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2f316b931ce2006975ad5277063f595fbf28d92e3230823e4e5bb9d9c5bc177c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57333976"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EducationAssignmentDefaults educationAssignmentDefaults = new EducationAssignmentDefaults();
educationAssignmentDefaults.addedStudentAction = EducationAddedStudentAction.ASSIGN_IF_OPEN;
educationAssignmentDefaults.notificationChannelUrl = "https://graph.microsoft.com/beta/teams('acdefc6b-2dc6-4e71-b1e9-6d9810ab1793')/channels('3da03fc4-8eac-4459-84fb-1422dc01f65e')";

graphClient.education().classes("acdefc6b-2dc6-4e71-b1e9-6d9810ab1793").assignmentDefaults()
    .buildRequest()
    .patch(educationAssignmentDefaults);

```