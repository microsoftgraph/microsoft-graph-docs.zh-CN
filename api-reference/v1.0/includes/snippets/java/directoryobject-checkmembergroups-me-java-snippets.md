---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bb7300cc9361bc6339b926fb9539ae09fbca22d3
ms.sourcegitcommit: e497ed9bb56400bdd2bb53d52ddf057d9966220b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/30/2021
ms.locfileid: "61224030"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<String> groupIdsList = new LinkedList<String>();
groupIdsList.add("fee2c45b-915a-4a64b130f4eb9e75525e");
groupIdsList.add("4fe90ae065a-478b9400e0a0e1cbd540");

graphClient.me()
    .checkMemberGroups(DirectoryObjectCheckMemberGroupsParameterSet
        .newBuilder()
        .withGroupIds(groupIdsList)
        .build())
    .buildRequest()
    .post();

```