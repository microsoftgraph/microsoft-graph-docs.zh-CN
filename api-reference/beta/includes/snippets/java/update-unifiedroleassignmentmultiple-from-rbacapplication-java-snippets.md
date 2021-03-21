---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b6fe13fd66b7934c2ad43f9c78a69167f8d898d6
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50975264"
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