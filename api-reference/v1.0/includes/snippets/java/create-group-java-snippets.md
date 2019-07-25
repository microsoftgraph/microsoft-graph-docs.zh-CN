---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: db6dbd4057f9a008a506c4151d64e779c861cfc6
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35893167"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Group group = new Group();
group.description = "Self help community for library";
group.displayName = "Library Assist";
LinkedList<String> groupTypesList = new LinkedList<String>();
groupTypesList.add("Unified");
group.groupTypes = groupTypesList;
group.mailEnabled = true;
group.mailNickname = "library";
group.securityEnabled = false;

graphClient.groups()
    .buildRequest()
    .post(group);

```