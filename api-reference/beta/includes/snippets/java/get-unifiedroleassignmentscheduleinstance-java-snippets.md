---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 119323224db0117079ab64edaf30c90af634f7b0235727b73927c8de01e148b2
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57332474"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

UnifiedRoleAssignmentScheduleInstance unifiedRoleAssignmentScheduleInstance = graphClient.roleManagement().directory().roleAssignmentScheduleInstances("eb18c026-c026-eb18-26c0-18eb26c018eb")
    .buildRequest()
    .get();

```