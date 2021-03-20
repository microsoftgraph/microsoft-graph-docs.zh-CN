---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f4bfe469c50bc8ed041d612944081f1b03dabf8d
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50973625"
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
group.visibility = "Private";

graphClient.groups()
    .buildRequest()
    .post(group);

```