---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1bbcd41a3ad7df7ee31ba00007051127f0d14d46e0bd9512a73b8764a9b2c751
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57278534"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

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