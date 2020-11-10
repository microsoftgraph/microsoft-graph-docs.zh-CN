---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a47236561dff964e23663fa6a3292726f2b35edd
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48978885"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

UnifiedRoleAssignmentMultiple unifiedRoleAssignmentMultiple = new UnifiedRoleAssignmentMultiple();
LinkedList<String> principalIdsList = new LinkedList<String>();
principalIdsList.add("0aeec2c1-fee7-4e02-b534-6f920d25b300");
principalIdsList.add("2d5386a7-732f-44db-9cf8-f82dd2a1c0e0");
unifiedRoleAssignmentMultiple.principalIds = principalIdsList;

graphClient.roleManagement().deviceManagement().roleAssignments("lAPpYvVpN0KRkAEhdxReEJC2sEqbR_9Hr48lds9SGHI-1")
    .buildRequest()
    .patch(unifiedRoleAssignmentMultiple);

```