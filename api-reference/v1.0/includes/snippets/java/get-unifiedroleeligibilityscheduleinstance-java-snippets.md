---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 410c04745784c1810f81669af02255616f88b40b
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65204888"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

UnifiedRoleEligibilityScheduleInstance unifiedRoleEligibilityScheduleInstance = graphClient.roleManagement().directory().roleEligibilityScheduleInstances("8MYkhImhnkm70CbBdTyW1BbHHAdHgZdDpbqyEFlRzAs-1-e")
    .buildRequest()
    .get();

```