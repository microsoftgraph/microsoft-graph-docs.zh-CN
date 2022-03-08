---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 655caf4f4b22e3cb405ce58775c1630bfbf6c7fb
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2022
ms.locfileid: "63338349"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<Option> requestOptions = new LinkedList<Option>();
requestOptions.add(new HeaderOption("ConsistencyLevel", "eventual"));

UnifiedRoleAssignmentCollectionPage transitiveRoleAssignments = graphClient.roleManagement().directory().transitiveRoleAssignments()
    .buildRequest( requestOptions )
    .filter("principalId eq '2c7936bc-3517-40f3-8eda-4806637b6516' and roleDefinitionId eq 'fe930be7-5e62-47db-91af-98c3a49a38b1'")
    .get();

```