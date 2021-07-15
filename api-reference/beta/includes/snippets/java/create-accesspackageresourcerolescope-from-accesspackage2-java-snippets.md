---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 40e869c2c219f6c4c923dccebe15d113baf88654
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/15/2021
ms.locfileid: "53439877"
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