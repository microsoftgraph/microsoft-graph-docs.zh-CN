---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2b7be748516a830c5c23c016c36da65092e1f8ac
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65204772"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

UnifiedRoleEligibilityScheduleRequestFilterByCurrentUserCollectionPage filterByCurrentUser = graphClient.roleManagement().directory().roleEligibilityScheduleRequests()
    .filterByCurrentUser(UnifiedRoleEligibilityScheduleRequestFilterByCurrentUserParameterSet
        .newBuilder()
        .withOn('principal')
        .build())
    .buildRequest()
    .get();

```