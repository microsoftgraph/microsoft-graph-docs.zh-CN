---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8c55f798dd6a5cbf0964a062ace5c1761b19e175406bf64f80f782ee49902c76
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57164138"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

UnifiedRoleAssignmentMultiple unifiedRoleAssignmentMultiple = new UnifiedRoleAssignmentMultiple();
unifiedRoleAssignmentMultiple.displayName = "NewName";
unifiedRoleAssignmentMultiple.description = "A new roleAssignment";

graphClient.roleManagement().cloudPC().roleAssignments("dbe9d288-fd87-41f4-b33d-b498ed207096")
    .buildRequest()
    .patch(unifiedRoleAssignmentMultiple);

```