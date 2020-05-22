---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3be13102635cfeec8f35e7236eacc4a1e890466e
ms.sourcegitcommit: 5a1373f2ccd9ee813fc60d42e7ac6b115b5f9f66
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/21/2020
ms.locfileid: "44338844"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Group group = new Group();
group.additionalDataManager().put("members@odata.bind", new JsonPrimitive("[
  "https://graph.microsoft.com/v1.0/directoryObjects/{id}",
  "https://graph.microsoft.com/v1.0/directoryObjects/{id}",
  "https://graph.microsoft.com/v1.0/directoryObjects/{id}"
]"));

graphClient.groups("{id}")
    .buildRequest()
    .patch(group);

```