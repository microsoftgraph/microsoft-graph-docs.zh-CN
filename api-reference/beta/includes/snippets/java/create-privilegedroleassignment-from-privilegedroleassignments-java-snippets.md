---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2112408be5c2935b366a8f4e72548b6f8b9cf03c
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48981957"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PrivilegedRoleAssignment privilegedRoleAssignment = new PrivilegedRoleAssignment();
privilegedRoleAssignment.userId = "userId-value";
privilegedRoleAssignment.roleId = "roleId-value";

graphClient.privilegedRoleAssignments()
    .buildRequest()
    .post(privilegedRoleAssignment);

```