---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c0dd46e4537f81b7fd2fd4b64431b4598f70c5d42f46843aa018903322be8d08
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57279459"
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