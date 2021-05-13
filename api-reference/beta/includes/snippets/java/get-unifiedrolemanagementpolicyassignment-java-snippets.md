---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 02624ba88aebec3423bd9c71f79a389c93e64a69
ms.sourcegitcommit: b8b0e88b3ba9a434dc45f5ab640cb46f66fae299
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/13/2021
ms.locfileid: "52474046"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

UnifiedRoleManagementPolicyAssignment unifiedRoleManagementPolicyAssignment = graphClient.policies().roleManagementPolicyAssignments("d6e4112f-112f-d6e4-2f11-e4d62f11e4d6")
    .buildRequest()
    .get();

```