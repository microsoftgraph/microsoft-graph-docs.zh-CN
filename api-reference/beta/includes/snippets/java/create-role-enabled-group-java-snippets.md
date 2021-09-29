---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 57c0c41f6589b5ba4f1f310ceaef47722f88da89
ms.sourcegitcommit: 36bae3615df41876493b25da478e589d1974f97b
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/29/2021
ms.locfileid: "59998182"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Group group = new Group();
group.description = "Group assignable to a role";
group.displayName = "Role assignable group";
LinkedList<String> groupTypesList = new LinkedList<String>();
groupTypesList.add("Unified");
group.groupTypes = groupTypesList;
group.isAssignableToRole = true;
group.mailEnabled = true;
group.securityEnabled = true;
group.mailNickname = "contosohelpdeskadministrators";
group.additionalDataManager().put("owners@odata.bind", new JsonPrimitive("[  \"https://graph.microsoft.com/beta/users/99e44b05-c10b-4e95-a523-e2732bbaba1e\"]"));
group.additionalDataManager().put("members@odata.bind", new JsonPrimitive("[  \"https://graph.microsoft.com/beta/users/6ea91a8d-e32e-41a1-b7bd-d2d185eed0e0\",  \"https://graph.microsoft.com/beta/users/4562bcc8-c436-4f95-b7c0-4f8ce89dca5e\"]"));

graphClient.groups()
    .buildRequest()
    .post(group);

```