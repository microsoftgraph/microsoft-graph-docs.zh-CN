---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 153244ee8b2abc3a9c96e1a009941f34d52968b1
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65206979"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

UnifiedRoleAssignment unifiedRoleAssignment = new UnifiedRoleAssignment();
unifiedRoleAssignment.principalId = "679a9213-c497-48a4-830a-8d3d25d94ddc";
unifiedRoleAssignment.roleDefinitionId = "ae79f266-94d4-4dab-b730-feca7e132178";
unifiedRoleAssignment.appScopeId = "/AccessPackageCatalog/beedadfe-01d5-4025-910b-84abb9369997";

graphClient.roleManagement().entitlementManagement().roleAssignments()
    .buildRequest()
    .post(unifiedRoleAssignment);

```