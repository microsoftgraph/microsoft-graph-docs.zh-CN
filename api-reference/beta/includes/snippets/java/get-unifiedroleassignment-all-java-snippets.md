---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 768223ff39e3bf4b8819368223a38865cc86f669
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2022
ms.locfileid: "63338354"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<Option> requestOptions = new LinkedList<Option>();
requestOptions.add(new HeaderOption("ConsistencyLevel", "eventual"));

UnifiedRoleAssignmentCollectionPage transitiveRoleAssignments = graphClient.roleManagement().directory().transitiveRoleAssignments()
    .buildRequest( requestOptions )
    .filter("principalId eq '2c7936bc-3517-40f3-8eda-4806637b6516'")
    .get();

```