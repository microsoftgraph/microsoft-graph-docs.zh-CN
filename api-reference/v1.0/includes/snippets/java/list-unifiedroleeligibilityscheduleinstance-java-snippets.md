---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4ee8a8e064d6264f0bd5f731354adced81b58a64
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65207074"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

UnifiedRoleEligibilityScheduleInstanceCollectionPage roleEligibilityScheduleInstances = graphClient.roleManagement().directory().roleEligibilityScheduleInstances()
    .buildRequest()
    .get();

```