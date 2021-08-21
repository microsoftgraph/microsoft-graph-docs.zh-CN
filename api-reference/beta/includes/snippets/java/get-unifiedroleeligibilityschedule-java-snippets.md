---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ffef1a047843f37dcb0bf6b4aba15c2f7bffff87ec76c125068d1a0ea768b268
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57105496"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

UnifiedRoleEligibilitySchedule unifiedRoleEligibilitySchedule = graphClient.roleManagement().directory().roleEligibilitySchedules("5cfd7709-7709-5cfd-0977-fd5c0977fd5c")
    .buildRequest()
    .get();

```