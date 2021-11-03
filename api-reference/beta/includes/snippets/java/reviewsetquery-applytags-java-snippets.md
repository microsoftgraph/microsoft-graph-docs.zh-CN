---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 44caf561c27c5a14d217fa570ef2ea2252ac671779d3dd39f6f1b70f21f1d2b1
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57105795"
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