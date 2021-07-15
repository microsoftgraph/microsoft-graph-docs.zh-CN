---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0438e2d47826a3dffc23d853ee290fd3d48e1a7d
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/15/2021
ms.locfileid: "53441289"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<UpdatableAsset> assetsList = new LinkedList<UpdatableAsset>();
AzureADDevice assets = new AzureADDevice();
assets.id = "String (identifier)";

assetsList.add(assets);
UpdatableAssetCollectionResponse updatableAssetCollectionResponse = new UpdatableAssetCollectionResponse();
updatableAssetCollectionResponse.value = assetsList;
UpdatableAssetCollectionPage updatableAssetCollectionPage = new UpdatableAssetCollectionPage(updatableAssetCollectionResponse, null);

graphClient.admin().windows().updates().updatableAssets("{updatableAssetGroupId}")
    .addMembers(UpdatableAssetAddMembersParameterSet
        .newBuilder()
        .withAssets(assetsList)
        .build())
    .buildRequest()
    .post();

```