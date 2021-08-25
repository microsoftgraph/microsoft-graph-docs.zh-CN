---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4283df452bf45a0a88d7cfbfcc7c6b4840837700
ms.sourcegitcommit: 9b8abc940a68dac6ee5da105ca29800cb59775f6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/25/2021
ms.locfileid: "58516064"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

UnifiedRoleAssignmentScheduleRequest unifiedRoleAssignmentScheduleRequest = graphClient.roleManagement().directory().roleAssignmentScheduleRequests("b5a22921-656a-4429-9c4e-59a5f576614d")
    .buildRequest()
    .get();

```