---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f5a617a7ed8318f902bf4f52b24a0a1eb58396ec
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/16/2019
ms.locfileid: "37544202"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Group group = new Group();
group.description = "Group with designated owner and members";
group.displayName = "Operations group";
LinkedList<String> groupTypesList = new LinkedList<String>();
groupTypesList.add("Unified");
group.groupTypes = groupTypesList;
group.mailEnabled = true;
group.mailNickname = "operations2019";
group.securityEnabled = false;
group.additionalDataManager().put("owners@odata.bind", new JsonPrimitive("[
  "https://graph.microsoft.com/v1.0/users/26be1845-4119-4801-a799-aea79d09f1a2"
]"));
group.additionalDataManager().put("members@odata.bind", new JsonPrimitive("[
  "https://graph.microsoft.com/v1.0/users/ff7cb387-6688-423c-8188-3da9532a73cc",
  "https://graph.microsoft.com/v1.0/users/69456242-0067-49d3-ba96-9de6f2728e14"
]"));

graphClient.groups()
    .buildRequest()
    .post(group);

```