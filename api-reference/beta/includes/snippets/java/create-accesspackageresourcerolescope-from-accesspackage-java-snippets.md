---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 65c08cd9862b7d088e51d94b866d38c0b6df559e
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48952318"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AccessPackageResourceRoleScope accessPackageResourceRoleScope = new AccessPackageResourceRoleScope();
AccessPackageResourceRole accessPackageResourceRole = new AccessPackageResourceRole();
accessPackageResourceRole.originId = "Member_b31fe1f1-3651-488f-bd9a-1711887fd4ca";
accessPackageResourceRole.displayName = "Member";
accessPackageResourceRole.originSystem = "AadGroup";
AccessPackageResource accessPackageResource = new AccessPackageResource();
accessPackageResource.id = "1d08498d-72a1-403f-8511-6b1f875746a0";
accessPackageResource.resourceType = "O365 Group";
accessPackageResource.originId = "b31fe1f1-3651-488f-bd9a-1711887fd4ca";
accessPackageResource.originSystem = "AadGroup";
accessPackageResourceRole.accessPackageResource = accessPackageResource;
accessPackageResourceRoleScope.accessPackageResourceRole = accessPackageResourceRole;
AccessPackageResourceScope accessPackageResourceScope = new AccessPackageResourceScope();
accessPackageResourceScope.originId = "b31fe1f1-3651-488f-bd9a-1711887fd4ca";
accessPackageResourceScope.originSystem = "AadGroup";
accessPackageResourceRoleScope.accessPackageResourceScope = accessPackageResourceScope;

graphClient.identityGovernance().entitlementManagement().accessPackages("{id}").accessPackageResourceRoleScopes()
    .buildRequest()
    .post(accessPackageResourceRoleScope);

```