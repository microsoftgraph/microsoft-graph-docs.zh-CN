---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0f9dc0c4e68cb07855385df8d1d00d217c611da6
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65205069"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

UnifiedRoleAssignmentScheduleRequest unifiedRoleAssignmentScheduleRequest = graphClient.roleManagement().directory().roleAssignmentScheduleRequests("95c690fb-3eb3-4942-a03f-4524aed6f31e")
    .buildRequest()
    .get();

```