---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: cff158311d13e31b57d03c4a2f4aa9b63c57af75e649cd1db58beba20bee526a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57332466"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

UpdateCategory updateCategory = UpdateCategory.FEATURE;

String memberEntityType = "#microsoft.graph.windowsUpdates.azureADDevice";

LinkedList<String> idsList = new LinkedList<String>();
idsList.add("String");
idsList.add("String");
idsList.add("String");

graphClient.admin().windows().updates().updatableAssets()
    .enrollAssetsById(UpdatableAssetEnrollAssetsByIdParameterSet
        .newBuilder()
        .withUpdateCategory(updateCategory)
        .withMemberEntityType(memberEntityType)
        .withIds(idsList)
        .build())
    .buildRequest()
    .post();

```