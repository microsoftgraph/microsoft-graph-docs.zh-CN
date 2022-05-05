---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3003f93a94b78323fbb05e7078190c1c152a2c46
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65205025"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

UnifiedRoleEligibilityScheduleFilterByCurrentUserCollectionPage filterByCurrentUser = graphClient.roleManagement().directory().roleEligibilitySchedules()
    .filterByCurrentUser(UnifiedRoleEligibilityScheduleFilterByCurrentUserParameterSet
        .newBuilder()
        .withOn('principal')
        .build())
    .buildRequest()
    .get();

```