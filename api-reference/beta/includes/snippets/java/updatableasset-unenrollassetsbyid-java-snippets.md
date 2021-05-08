---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e17ae4d879e3a20b287f95e15d5518ebb312b849
ms.sourcegitcommit: 2a35434fabc76672e21bfc3ed5a1d28f9f3b66bc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2021
ms.locfileid: "52240689"
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
    .unenrollAssetsById(UpdatableAssetUnenrollAssetsByIdParameterSet
        .newBuilder()
        .withUpdateCategory(updateCategory)
        .withMemberEntityType(memberEntityType)
        .withIds(idsList)
        .build())
    .buildRequest()
    .post();

```