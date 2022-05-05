---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 94fd4367d14220d6e1c72cb075f88dc8a993769c
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65205283"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

UnifiedRoleAssignmentScheduleInstanceFilterByCurrentUserCollectionPage filterByCurrentUser = graphClient.roleManagement().directory().roleAssignmentScheduleInstances()
    .filterByCurrentUser(UnifiedRoleAssignmentScheduleInstanceFilterByCurrentUserParameterSet
        .newBuilder()
        .withOn('principal')
        .build())
    .buildRequest()
    .get();

```