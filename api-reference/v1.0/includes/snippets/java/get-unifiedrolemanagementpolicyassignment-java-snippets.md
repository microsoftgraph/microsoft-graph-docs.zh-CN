---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 57657b2218b1a49b61cc2a0ff9455dfa10d7ea03
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65204509"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

UnifiedRoleManagementPolicyAssignment unifiedRoleManagementPolicyAssignment = graphClient.policies().roleManagementPolicyAssignments("Directory_cab01047-8ad9-4792-8e42-569340767f1b_70c808b5-0d35-4863-a0ba-07888e99d448_62e90394-69f5-4237-9190-012177145e10")
    .buildRequest()
    .get();

```