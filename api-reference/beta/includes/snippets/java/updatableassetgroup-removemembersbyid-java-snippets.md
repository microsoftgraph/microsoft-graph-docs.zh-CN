---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7d08a77c2184d407cb5d81a445753862d9cb9a10
ms.sourcegitcommit: 2a35434fabc76672e21bfc3ed5a1d28f9f3b66bc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2021
ms.locfileid: "52239041"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<String> idsList = new LinkedList<String>();
idsList.add("String");
idsList.add("String");
idsList.add("String");

String memberEntityType = "#microsoft.graph.windowsUpdates.azureADDevice";

graphClient.admin().windows().updates().updatableAssets("{updatableAssetGroupId}")
    .removeMembersById(UpdatableAssetRemoveMembersByIdParameterSet
        .newBuilder()
        .withIds(idsList)
        .withMemberEntityType(memberEntityType)
        .build())
    .buildRequest()
    .post();

```