---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c9bbe203c7cce861b63434b44c899cb9df44f758
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50979835"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Group group = new Group();
group.description = "description-value";
group.displayName = "displayName-value";
LinkedList<String> groupTypesList = new LinkedList<String>();
groupTypesList.add("groupTypes-value");
group.groupTypes = groupTypesList;
group.mail = "mail-value";
group.mailEnabled = true;
group.mailNickname = "mailNickname-value";

graphClient.groups("{id}")
    .buildRequest()
    .patch(group);

```