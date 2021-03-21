---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d41971c3d53e07e178218535fb23f7f1813671fd
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50982035"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<Tag> tagsToAddList = new LinkedList<Tag>();
Tag tagsToAdd = new Tag();
tagsToAdd.id = "b4798d14-748d-468e-a1ec-96a2b1d49677";

tagsToAddList.add(tagsToAdd);
TagCollectionResponse tagCollectionResponse = new TagCollectionResponse();
tagCollectionResponse.value = tagsToAddList;
TagCollectionPage tagCollectionPage = new TagCollectionPage(tagCollectionResponse, null);

graphClient.compliance().ediscovery().cases("47746044-fd0b-4a30-acfc-5272b691ba5b").reviewSets("6c95c2a6-31fa-45a8-93ef-dd4531974783").queries("b4798d14-748d-468e-a1ec-96a2b1d49677")
    .applyTags(ReviewSetQueryApplyTagsParameterSet
        .newBuilder()
        .withTagsToAdd(tagsToAddList)
        .withTagsToRemove(null)
        .build())
    .buildRequest()
    .post();

```