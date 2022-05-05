---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9d508a93d44164b3f16757a1e5dd8b49b529c6d5
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65205358"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

UnifiedRoleAssignmentSchedule unifiedRoleAssignmentSchedule = graphClient.roleManagement().directory().roleAssignmentSchedules("95c690fb-3eb3-4942-a03f-4524aed6f31e")
    .buildRequest()
    .get();

```