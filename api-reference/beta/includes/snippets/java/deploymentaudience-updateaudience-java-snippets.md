---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6383d29afc2dc7725c295d88ca432d8ba885b0e7
ms.sourcegitcommit: 2a35434fabc76672e21bfc3ed5a1d28f9f3b66bc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2021
ms.locfileid: "52241274"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<UpdatableAsset> addMembersList = new LinkedList<UpdatableAsset>();
UpdatableAsset addMembers = new UpdatableAsset();
addMembers.id = "String (identifier)";

addMembersList.add(addMembers);
UpdatableAssetCollectionResponse updatableAssetCollectionResponse = new UpdatableAssetCollectionResponse();
updatableAssetCollectionResponse.value = addMembersList;
UpdatableAssetCollectionPage updatableAssetCollectionPage = new UpdatableAssetCollectionPage(updatableAssetCollectionResponse, null);

LinkedList<UpdatableAsset> removeMembersList = new LinkedList<UpdatableAsset>();
UpdatableAsset removeMembers = new UpdatableAsset();
removeMembers.id = "String (identifier)";

removeMembersList.add(removeMembers);
UpdatableAssetCollectionResponse updatableAssetCollectionResponse = new UpdatableAssetCollectionResponse();
updatableAssetCollectionResponse.value = removeMembersList;
UpdatableAssetCollectionPage updatableAssetCollectionPage = new UpdatableAssetCollectionPage(updatableAssetCollectionResponse, null);

LinkedList<UpdatableAsset> addExclusionsList = new LinkedList<UpdatableAsset>();
UpdatableAsset addExclusions = new UpdatableAsset();
addExclusions.id = "String (identifier)";

addExclusionsList.add(addExclusions);
UpdatableAssetCollectionResponse updatableAssetCollectionResponse = new UpdatableAssetCollectionResponse();
updatableAssetCollectionResponse.value = addExclusionsList;
UpdatableAssetCollectionPage updatableAssetCollectionPage = new UpdatableAssetCollectionPage(updatableAssetCollectionResponse, null);

LinkedList<UpdatableAsset> removeExclusionsList = new LinkedList<UpdatableAsset>();
UpdatableAsset removeExclusions = new UpdatableAsset();
removeExclusions.id = "String (identifier)";

removeExclusionsList.add(removeExclusions);
UpdatableAssetCollectionResponse updatableAssetCollectionResponse = new UpdatableAssetCollectionResponse();
updatableAssetCollectionResponse.value = removeExclusionsList;
UpdatableAssetCollectionPage updatableAssetCollectionPage = new UpdatableAssetCollectionPage(updatableAssetCollectionResponse, null);

graphClient.admin().windows().updates().deployments("{deploymentId}").audience()
    .updateAudience(DeploymentAudienceUpdateAudienceParameterSet
        .newBuilder()
        .withAddMembers(addMembersList)
        .withRemoveMembers(removeMembersList)
        .withAddExclusions(addExclusionsList)
        .withRemoveExclusions(removeExclusionsList)
        .build())
    .buildRequest()
    .post();

```