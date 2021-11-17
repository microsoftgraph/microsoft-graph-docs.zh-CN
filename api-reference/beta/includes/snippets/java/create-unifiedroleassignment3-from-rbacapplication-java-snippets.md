---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6862e4f7c8105e2b4f7f31850043335c2aab4140c1e64bfadb8f98f1855910a1
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57106866"
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