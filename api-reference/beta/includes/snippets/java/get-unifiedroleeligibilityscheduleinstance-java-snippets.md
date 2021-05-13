---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d3fc19c292c5d23e2825aee48e63126dc9e4e8e6
ms.sourcegitcommit: b8b0e88b3ba9a434dc45f5ab640cb46f66fae299
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/13/2021
ms.locfileid: "52474522"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

UnifiedRoleEligibilityScheduleInstance unifiedRoleEligibilityScheduleInstance = graphClient.roleManagement().directory().roleEligibilityScheduleInstances("5cfd7709-7709-5cfd-0977-fd5c0977fd5c")
    .buildRequest()
    .get();

```