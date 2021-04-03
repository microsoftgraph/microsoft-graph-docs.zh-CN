---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d05a3c7ae352c48f0da6cfc67eee378dc2931861
ms.sourcegitcommit: 08d47a31c48fd69ae4fcee26e34fdd65ad1ba69f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/02/2021
ms.locfileid: "51573180"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

SourceCollection sourceCollection = new SourceCollection();
sourceCollection.id = "1a9b4145d8f84e39bc45a7f68c5c5119";

EnumSet<AdditionalDataOptions> additionalData = EnumSet.of(AdditionalDataOptions.LINKED_FILES);

graphClient.compliance().ediscovery().cases("080e8cad-f21f-4452-8826-0ddf7e949fdd").reviewSets("6fe25d32-8167-4625-b75c-c4181ccbd9d5")
    .addToReviewSet(ReviewSetAddToReviewSetParameterSet
        .newBuilder()
        .withSourceCollection(sourceCollection)
        .withAdditionalData(additionalData)
        .build())
    .buildRequest()
    .post();

```