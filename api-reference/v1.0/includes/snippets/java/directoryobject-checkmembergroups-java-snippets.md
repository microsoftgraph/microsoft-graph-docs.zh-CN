---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 759563b0cd0b011f9d149ec483db136f554136fc
ms.sourcegitcommit: e497ed9bb56400bdd2bb53d52ddf057d9966220b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/30/2021
ms.locfileid: "61224019"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<String> groupIdsList = new LinkedList<String>();
groupIdsList.add("f448435d-3ca7-4073-8152-a1fd73c0fd09");
groupIdsList.add("bd7c6263-4dd5-4ae8-8c96-556e1c0bece6");
groupIdsList.add("93670da6-d731-4366-94b5-abed40b6016b");
groupIdsList.add("f5484ab1-4d4d-41ec-a9b8-754b3957bfc7");
groupIdsList.add("c9103f26-f3cf-4004-a611-2a14e81b8f79");

graphClient.directoryObjects("4562bcc8-c436-4f95-b7c0-4f8ce89dca5e")
    .checkMemberGroups(DirectoryObjectCheckMemberGroupsParameterSet
        .newBuilder()
        .withGroupIds(groupIdsList)
        .build())
    .buildRequest()
    .post();

```