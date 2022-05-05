---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 36fa85c9c0e457df4d42002e23c9c944fdd97282
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65207354"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

UnifiedRoleManagementPolicyAssignmentCollectionPage roleManagementPolicyAssignments = graphClient.policies().roleManagementPolicyAssignments()
    .buildRequest()
    .filter("scopeId eq '/' and scopeType eq 'Directory'")
    .get();

```