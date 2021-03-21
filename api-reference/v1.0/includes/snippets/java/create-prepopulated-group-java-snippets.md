---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a5f296007e0c15059ed9a5fc0921b7bfd209add0
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50980734"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Group group = new Group();
group.description = "Group with designated owner and members";
group.displayName = "Operations group";
LinkedList<String> groupTypesList = new LinkedList<String>();
group.groupTypes = groupTypesList;
group.mailEnabled = false;
group.mailNickname = "operations2019";
group.securityEnabled = true;
group.additionalDataManager().put("owners@odata.bind", new JsonPrimitive("[  \"https://graph.microsoft.com/v1.0/users/26be1845-4119-4801-a799-aea79d09f1a2\"]"));
group.additionalDataManager().put("members@odata.bind", new JsonPrimitive("[  \"https://graph.microsoft.com/v1.0/users/ff7cb387-6688-423c-8188-3da9532a73cc\",  \"https://graph.microsoft.com/v1.0/users/69456242-0067-49d3-ba96-9de6f2728e14\"]"));

graphClient.groups()
    .buildRequest()
    .post(group);

```