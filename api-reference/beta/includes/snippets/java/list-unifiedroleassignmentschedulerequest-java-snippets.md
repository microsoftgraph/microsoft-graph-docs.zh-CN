---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ce82ceefebc0619b61d8984604aba7ab06bb0b38
ms.sourcegitcommit: b8b0e88b3ba9a434dc45f5ab640cb46f66fae299
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/13/2021
ms.locfileid: "52474578"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

UnifiedRoleAssignmentScheduleRequestCollectionPage roleAssignmentScheduleRequests = graphClient.roleManagement().directory().roleAssignmentScheduleRequests()
    .buildRequest()
    .get();

```