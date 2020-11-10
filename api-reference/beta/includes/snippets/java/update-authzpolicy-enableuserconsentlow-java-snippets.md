---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: aaf24b1aff8d671336a0af0fb6a63b09977ecb3f
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48961450"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AuthorizationPolicy authorizationPolicy = new AuthorizationPolicy();
LinkedList<String> permissionGrantPolicyIdsAssignedToDefaultUserRoleList = new LinkedList<String>();
permissionGrantPolicyIdsAssignedToDefaultUserRoleList.add("managePermissionGrantsForSelf.microsoft-user-default-low");
authorizationPolicy.permissionGrantPolicyIdsAssignedToDefaultUserRole = permissionGrantPolicyIdsAssignedToDefaultUserRoleList;

graphClient.policies().authorizationPolicy("authorizationPolicy")
    .buildRequest()
    .patch(authorizationPolicy);

```