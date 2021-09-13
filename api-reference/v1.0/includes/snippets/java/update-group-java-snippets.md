---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f3e2ccfe275cd99ceac9b66414c54080660b55cdb529fa7b21e1f563fb39330c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57162581"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Group group = new Group();
group.description = "Library Assist";
group.displayName = "Library Assist";
LinkedList<String> groupTypesList = new LinkedList<String>();
groupTypesList.add("Unified");
group.groupTypes = groupTypesList;
group.mailEnabled = true;
group.mailNickname = "library-help";

graphClient.groups("{id}")
    .buildRequest()
    .patch(group);

```