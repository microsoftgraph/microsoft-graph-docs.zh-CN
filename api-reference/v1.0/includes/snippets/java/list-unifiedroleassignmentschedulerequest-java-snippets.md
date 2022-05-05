---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ce82ceefebc0619b61d8984604aba7ab06bb0b38
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65207235"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

UnifiedRoleAssignmentScheduleRequestCollectionPage roleAssignmentScheduleRequests = graphClient.roleManagement().directory().roleAssignmentScheduleRequests()
    .buildRequest()
    .get();

```