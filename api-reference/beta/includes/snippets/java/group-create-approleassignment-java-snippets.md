---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 92e99891e19eb47983b63fe18174fd99f643ccc4
ms.sourcegitcommit: 9a5facff47a8d4e05ecd2c6cd68294a948c47c4d
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2021
ms.locfileid: "49945533"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AppRoleAssignment appRoleAssignment = new AppRoleAssignment();
appRoleAssignment.principalId = UUID.fromString("principalId-value");
appRoleAssignment.resourceId = UUID.fromString("resourceId-value");
appRoleAssignment.appRoleId = UUID.fromString("appRoleId-value");

graphClient.groups("{id}").appRoleAssignments()
    .buildRequest()
    .post(appRoleAssignment);

```