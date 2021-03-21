---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e6b42a1bac35d40133a6f847e6cc3afe5adace93
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50978478"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<String> groupIdsList = new LinkedList<String>();
groupIdsList.add("fee2c45b-915a-4a64b130f4eb9e75525e");
groupIdsList.add("4fe90ae065a-478b9400e0a0e1cbd540");

graphClient.directoryObjects("{id}")
    .checkMemberGroups(DirectoryObjectCheckMemberGroupsParameterSet
        .newBuilder()
        .withGroupIds(groupIdsList)
        .build())
    .buildRequest()
    .post();

```