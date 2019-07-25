---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5eef34c761e46e16e5d40131c5225763e595b5a0
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35893168"
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
group.additionalDataManager().put("owners@odata.bind", new JsonPrimitive(["https://graph.microsoft.com/v1.0/users/26be1845-4119-4801-a799-aea79d09f1a2"]));
group.additionalDataManager().put("members@odata.bind", new JsonPrimitive(["https://graph.microsoft.com/v1.0/users/ff7cb387-6688-423c-8188-3da9532a73cc","https://graph.microsoft.com/v1.0/users/69456242-0067-49d3-ba96-9de6f2728e14"]));

graphClient.groups()
    .buildRequest()
    .post(group);

```