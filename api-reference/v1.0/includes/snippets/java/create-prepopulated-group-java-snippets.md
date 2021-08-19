---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5078efd269c85f6b254d841cf76a14358d67a100559488b11244a9a4dfbdb4c1
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57278540"
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