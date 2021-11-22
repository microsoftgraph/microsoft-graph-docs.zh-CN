---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 49e154023ced1cee68d2e3a3f463c37160275c6e1d188c0fcc194c9c88372d47
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57274117"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<String> idsList = new LinkedList<String>();
idsList.add("String");
idsList.add("String");
idsList.add("String");

String memberEntityType = "#microsoft.graph.windowsUpdates.azureADDevice";

graphClient.admin().windows().updates().updatableAssets("{updatableAssetGroupId}")
    .addMembersById(UpdatableAssetAddMembersByIdParameterSet
        .newBuilder()
        .withIds(idsList)
        .withMemberEntityType(memberEntityType)
        .build())
    .buildRequest()
    .post();

```