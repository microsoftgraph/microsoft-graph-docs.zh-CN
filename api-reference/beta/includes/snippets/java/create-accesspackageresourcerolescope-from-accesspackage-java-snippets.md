---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4d528570bd3b38198ddb9105e42c57559b7d1487f53f38fe81a1d6c4f8a1094d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56902831"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

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