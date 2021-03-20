---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 622e2fc0a5f271875ececc25a558d1cd0d3a1d5d
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50968449"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Group group = new Group();
group.description = "Self help community for golf";
group.displayName = "Golf Assist";
LinkedList<String> groupTypesList = new LinkedList<String>();
groupTypesList.add("Unified");
group.groupTypes = groupTypesList;
group.mailEnabled = true;
group.mailNickname = "golfassist";
group.securityEnabled = false;

graphClient.groups()
    .buildRequest()
    .post(group);

```