---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 64a74800d526ba18af496c11f2e72d1a758ecdcc
ms.sourcegitcommit: 9b8abc940a68dac6ee5da105ca29800cb59775f6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/25/2021
ms.locfileid: "58516048"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

UnifiedRoleAssignmentScheduleInstance unifiedRoleAssignmentScheduleInstance = graphClient.roleManagement().directory().roleAssignmentScheduleInstances("4-PYiFWPHkqVOpuYmLiHa_8KmpPnrkhHmG41_UYRbUY-1")
    .buildRequest()
    .get();

```