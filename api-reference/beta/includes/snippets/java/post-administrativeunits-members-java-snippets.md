---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 27693309fbb7a63fe9900fca838c0724749834ab
ms.sourcegitcommit: c6a8c1cc13ace38d6c4371139ee84707c5c93352
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2021
ms.locfileid: "60890215"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Group directoryObject = new Group();
directoryObject.description = "Self help community for golf";
directoryObject.displayName = "Golf Assist";
LinkedList<String> groupTypesList = new LinkedList<String>();
groupTypesList.add("Unified");
directoryObject.groupTypes = groupTypesList;
directoryObject.mailEnabled = true;
directoryObject.mailNickname = "golfassist";
directoryObject.securityEnabled = false;

graphClient.administrativeUnits("{id}").members()
    .buildRequest()
    .post(directoryObject);

```