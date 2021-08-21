---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9a65f87b3cc61834cc46dbe1863cdf73b087b85ce464260792b539efbd5ad2d1
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56903276"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

UnifiedRoleAssignmentScheduleCollectionPage roleAssignmentSchedules = graphClient.roleManagement().directory().roleAssignmentSchedules()
    .buildRequest()
    .get();

```