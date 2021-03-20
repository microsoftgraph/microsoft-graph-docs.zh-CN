---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2ef671398edd2ea58d2ff15355aabb2cdb443e85
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50974959"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

SourceCollection sourceCollection = new SourceCollection();
sourceCollection.id = "1a9b4145d8f84e39bc45a7f68c5c5119";

EnumSet<DataCollectionScope> additionalData = EnumSet.of(DataCollectionScope.LINKED_FILES);

graphClient.compliance().ediscovery().cases("080e8cad-f21f-4452-8826-0ddf7e949fdd").reviewSets("6fe25d32-8167-4625-b75c-c4181ccbd9d5")
    .addToReviewSet(ReviewSetAddToReviewSetParameterSet
        .newBuilder()
        .withSourceCollection(sourceCollection)
        .withAdditionalData(additionalData)
        .build())
    .buildRequest()
    .post();

```