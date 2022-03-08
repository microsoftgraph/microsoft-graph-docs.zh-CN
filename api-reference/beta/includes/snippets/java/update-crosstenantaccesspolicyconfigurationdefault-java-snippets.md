---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f75d3dabf1953fe100264efb0dcc8fc3bffbf62b
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2022
ms.locfileid: "63335526"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

CrossTenantAccessPolicyConfigurationDefault crossTenantAccessPolicyConfigurationDefault = new CrossTenantAccessPolicyConfigurationDefault();
CrossTenantAccessPolicyB2BSetting b2bCollaborationOutbound = new CrossTenantAccessPolicyB2BSetting();
CrossTenantAccessPolicyTargetConfiguration usersAndGroups = new CrossTenantAccessPolicyTargetConfiguration();
usersAndGroups.accessType = CrossTenantAccessPolicyTargetConfigurationAccessType.BLOCKED;
LinkedList<CrossTenantAccessPolicyTarget> targetsList = new LinkedList<CrossTenantAccessPolicyTarget>();
CrossTenantAccessPolicyTarget targets = new CrossTenantAccessPolicyTarget();
targets.target = "0be493dc-cb56-4a53-936f-9cf64410b8b0";
targets.targetType = CrossTenantAccessPolicyTargetType.GROUP;
targetsList.add(targets);
usersAndGroups.targets = targetsList;
b2bCollaborationOutbound.usersAndGroups = usersAndGroups;
CrossTenantAccessPolicyTargetConfiguration applications = new CrossTenantAccessPolicyTargetConfiguration();
applications.accessType = CrossTenantAccessPolicyTargetConfigurationAccessType.BLOCKED;
LinkedList<CrossTenantAccessPolicyTarget> targetsList1 = new LinkedList<CrossTenantAccessPolicyTarget>();
CrossTenantAccessPolicyTarget targets1 = new CrossTenantAccessPolicyTarget();
targets1.target = "AllApplications";
targets1.targetType = CrossTenantAccessPolicyTargetType.APPLICATION;
targetsList1.add(targets1);
applications.targets = targetsList1;
b2bCollaborationOutbound.applications = applications;
crossTenantAccessPolicyConfigurationDefault.b2bCollaborationOutbound = b2bCollaborationOutbound;

graphClient.policies().crossTenantAccessPolicy().default()
    .buildRequest()
    .patch(crossTenantAccessPolicyConfigurationDefault);

```