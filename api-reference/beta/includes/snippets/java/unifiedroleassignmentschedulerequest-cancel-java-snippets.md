---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ab2363712ec6214dfae4a44e633597372c20be94
ms.sourcegitcommit: b8b0e88b3ba9a434dc45f5ab640cb46f66fae299
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/13/2021
ms.locfileid: "52475096"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.roleManagement().directory().roleAssignmentScheduleRequests("{unifiedRoleAssignmentScheduleRequestsId}")
    .cancel()
    .buildRequest()
    .post();

```