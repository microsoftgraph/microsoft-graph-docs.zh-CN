---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f981c88b8df1abb66aa7c0b8519252f036ca4006
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/15/2021
ms.locfileid: "53442692"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

UnifiedRoleAssignmentScheduleInstance unifiedRoleAssignmentScheduleInstance = graphClient.roleManagement().directory().roleAssignmentScheduleInstances("eb18c026-c026-eb18-26c0-18eb26c018eb")
    .buildRequest()
    .get();

```