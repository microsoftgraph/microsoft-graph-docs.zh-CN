---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 06ccf6dd188fe9bb3676d2581fee0354cd555b8805b30c1a13fdc5db048550d2
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57277733"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

UnifiedRoleAssignmentMultiple unifiedRoleAssignmentMultiple = new UnifiedRoleAssignmentMultiple();
LinkedList<String> principalIdsList = new LinkedList<String>();
principalIdsList.add("0aeec2c1-fee7-4e02-b534-6f920d25b300");
principalIdsList.add("2d5386a7-732f-44db-9cf8-f82dd2a1c0e0");
unifiedRoleAssignmentMultiple.principalIds = principalIdsList;

graphClient.roleManagement().deviceManagement().roleAssignments("lAPpYvVpN0KRkAEhdxReEJC2sEqbR_9Hr48lds9SGHI-1")
    .buildRequest()
    .patch(unifiedRoleAssignmentMultiple);

```