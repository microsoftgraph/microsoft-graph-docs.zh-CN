---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a2643cf94b4685ba7c510ce1c279ccb982add9d38f5f9de370086de2a61678a9
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57104217"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AccessPackageResourceRoleScope accessPackageResourceRoleScope = new AccessPackageResourceRoleScope();
AccessPackageResourceRole accessPackageResourceRole = new AccessPackageResourceRole();
accessPackageResourceRole.originId = "4";
accessPackageResourceRole.originSystem = "SharePointOnline";
AccessPackageResource accessPackageResource = new AccessPackageResource();
accessPackageResource.id = "53c71803-a0a8-4777-aecc-075de8ee3991";
accessPackageResourceRole.accessPackageResource = accessPackageResource;
accessPackageResourceRoleScope.accessPackageResourceRole = accessPackageResourceRole;
AccessPackageResourceScope accessPackageResourceScope = new AccessPackageResourceScope();
accessPackageResourceScope.id = "5ae0ae7c-d0a5-42aa-ab37-1f15e9a61d33";
accessPackageResourceScope.originId = "https://microsoft.sharepoint.com/portals/Community";
accessPackageResourceScope.originSystem = "SharePointOnline";
accessPackageResourceRoleScope.accessPackageResourceScope = accessPackageResourceScope;

graphClient.identityGovernance().entitlementManagement().accessPackages("{id}").accessPackageResourceRoleScopes()
    .buildRequest()
    .post(accessPackageResourceRoleScope);

```