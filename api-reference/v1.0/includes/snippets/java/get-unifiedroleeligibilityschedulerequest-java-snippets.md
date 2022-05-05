---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: aed3381f53879aebcf427bf2cc687eb0e910833a
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65204735"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

UnifiedRoleEligibilityScheduleRequest unifiedRoleEligibilityScheduleRequest = graphClient.roleManagement().directory().roleEligibilityScheduleRequests("f341269e-c926-41fa-a905-cef3b01b2a67")
    .buildRequest()
    .get();

```