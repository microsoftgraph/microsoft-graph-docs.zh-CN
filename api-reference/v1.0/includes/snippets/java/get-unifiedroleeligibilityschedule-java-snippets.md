---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 82d2dc1da406b7b6a1a209710b745cdf4dc11cb7
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65204987"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

UnifiedRoleEligibilitySchedule unifiedRoleEligibilitySchedule = graphClient.roleManagement().directory().roleEligibilitySchedules("1f06eafc-7532-429b-abf1-ab5a5f4a7052")
    .buildRequest()
    .get();

```