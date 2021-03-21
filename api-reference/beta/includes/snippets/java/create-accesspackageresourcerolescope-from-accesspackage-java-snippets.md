---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 96ae5c7e6a93a9d30f39366ec374c1de9274cacf
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50982624"
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