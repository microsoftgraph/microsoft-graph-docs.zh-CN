---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 38f0b21c6181f136c6b8e60748ec4b4d5b9c820f
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/15/2021
ms.locfileid: "53442867"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

UpdateCategory updateCategory = UpdateCategory.FEATURE;

LinkedList<UpdatableAsset> assetsList = new LinkedList<UpdatableAsset>();
AzureADDevice assets = new AzureADDevice();
assets.id = "String (identifier)";

assetsList.add(assets);
UpdatableAssetCollectionResponse updatableAssetCollectionResponse = new UpdatableAssetCollectionResponse();
updatableAssetCollectionResponse.value = assetsList;
UpdatableAssetCollectionPage updatableAssetCollectionPage = new UpdatableAssetCollectionPage(updatableAssetCollectionResponse, null);

graphClient.admin().windows().updates().updatableAssets()
    .unenrollAssets(UpdatableAssetUnenrollAssetsParameterSet
        .newBuilder()
        .withUpdateCategory(updateCategory)
        .withAssets(assetsList)
        .build())
    .buildRequest()
    .post();

```