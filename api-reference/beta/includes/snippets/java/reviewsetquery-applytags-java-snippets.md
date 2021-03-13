---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7b58b2d60aa4d6c72cf05071c26c698d594936ae
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50772834"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<Tag> tagsToAddList = new LinkedList<Tag>();
Tag tagsToAdd = new Tag();
tagsToAdd.id = "b4798d14-748d-468e-a1ec-96a2b1d49677";

tagsToAddList.add(tagsToAdd);
TagCollectionResponse tagCollectionResponse = new TagCollectionResponse();
tagCollectionResponse.value = tagsToAddList;
TagCollectionPage tagCollectionPage = new TagCollectionPage(tagCollectionResponse, null);

graphClient.compliance().ediscovery().cases("47746044-fd0b-4a30-acfc-5272b691ba5b").reviewSets("6c95c2a6-31fa-45a8-93ef-dd4531974783").queries("b4798d14-748d-468e-a1ec-96a2b1d49677")
    .applyTags(tagsToAddList,null)
    .buildRequest()
    .post();

```