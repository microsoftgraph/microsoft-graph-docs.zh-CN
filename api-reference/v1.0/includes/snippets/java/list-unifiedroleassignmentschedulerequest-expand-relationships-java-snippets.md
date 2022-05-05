---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bbc87e6795456a1f15997be35e125be0576f6a39
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65207267"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

UnifiedRoleAssignmentScheduleRequestCollectionPage roleAssignmentScheduleRequests = graphClient.roleManagement().directory().roleAssignmentScheduleRequests()
    .buildRequest()
    .expand("roleDefinitionId")
    .select("principalId,action,roleDefinitionId")
    .get();

```