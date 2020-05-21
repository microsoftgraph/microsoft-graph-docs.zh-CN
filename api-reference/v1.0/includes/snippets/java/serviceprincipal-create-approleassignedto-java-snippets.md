---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f3d8dd3cee4fcb7df148e53192db4907676e25d4
ms.sourcegitcommit: 5a1373f2ccd9ee813fc60d42e7ac6b115b5f9f66
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/21/2020
ms.locfileid: "44335051"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AppRoleAssignment appRoleAssignment = new AppRoleAssignment();
appRoleAssignment.principalId = "principalId-value";
appRoleAssignment.resourceId = "resourceId-value";
appRoleAssignment.appRoleId = "appRoleId-value";

graphClient.servicePrincipals("{id}").appRoleAssignedTo()
    .buildRequest()
    .post(appRoleAssignment);

```