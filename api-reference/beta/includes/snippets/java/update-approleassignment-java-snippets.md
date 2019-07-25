---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 6d18bf8895000882a7b0722a7c69678b07806512
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35856631"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AppRoleAssignment appRoleAssignment = new AppRoleAssignment();
appRoleAssignment.creationTimestamp = "2016-10-19T10:37:00Z";
appRoleAssignment.principalDisplayName = "principalDisplayName-value";
appRoleAssignment.principalId = "principalId-value";
appRoleAssignment.principalType = "principalType-value";
appRoleAssignment.resourceDisplayName = "resourceDisplayName-value";

graphClient.appRoleAssignments("{id}")
    .buildRequest()
    .patch(appRoleAssignment);

```