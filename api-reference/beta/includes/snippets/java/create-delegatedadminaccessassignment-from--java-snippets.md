---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 18ec97280b9ae4343539b411a110f7a7d2b68024
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65210800"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DelegatedAdminAccessAssignment delegatedAdminAccessAssignment = new DelegatedAdminAccessAssignment();
DelegatedAdminAccessContainer accessContainer = new DelegatedAdminAccessContainer();
accessContainer.accessContainerId = "869713c9-0b28-4d08-8949-ae07ae1bf528";
accessContainer.accessContainerType = DelegatedAdminAccessContainerType.SECURITY_GROUP;
delegatedAdminAccessAssignment.accessContainer = accessContainer;
DelegatedAdminAccessDetails accessDetails = new DelegatedAdminAccessDetails();
LinkedList<UnifiedRole> unifiedRolesList = new LinkedList<UnifiedRole>();
UnifiedRole unifiedRoles = new UnifiedRole();
unifiedRoles.roleDefinitionId = "29232cdf-9323-42fd-ade2-1d097af3e4de";
unifiedRolesList.add(unifiedRoles);
UnifiedRole unifiedRoles1 = new UnifiedRole();
unifiedRoles1.roleDefinitionId = "f2ef992c-3afb-46b9-b7cf-a126ee74c451";
unifiedRolesList.add(unifiedRoles1);
UnifiedRole unifiedRoles2 = new UnifiedRole();
unifiedRoles2.roleDefinitionId = "729827e3-9c14-49f7-bb1b-9608f156bbb8";
unifiedRolesList.add(unifiedRoles2);
UnifiedRole unifiedRoles3 = new UnifiedRole();
unifiedRoles3.roleDefinitionId = "3a2c62db-5318-420d-8d74-23affee5d9d5";
unifiedRolesList.add(unifiedRoles3);
accessDetails.unifiedRoles = unifiedRolesList;
delegatedAdminAccessAssignment.accessDetails = accessDetails;

graphClient.tenantRelationships().delegatedAdminRelationships("72a7ae7e-4887-4e34-9755-2e1e9b26b943-63f017cb-9e0d-4f14-94bd-4871902b3409").accessAssignments()
    .buildRequest()
    .post(delegatedAdminAccessAssignment);

```