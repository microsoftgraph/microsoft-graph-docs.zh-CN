---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ded579acf29f1824a5c78c55b9c0d5751c917de7
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65205337"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

UnifiedRoleAssignmentScheduleFilterByCurrentUserCollectionPage filterByCurrentUser = graphClient.roleManagement().directory().roleAssignmentSchedules()
    .filterByCurrentUser(UnifiedRoleAssignmentScheduleFilterByCurrentUserParameterSet
        .newBuilder()
        .withOn('principal')
        .build())
    .buildRequest()
    .get();

```