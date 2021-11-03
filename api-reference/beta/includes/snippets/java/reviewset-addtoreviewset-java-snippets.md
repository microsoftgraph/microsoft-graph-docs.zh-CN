---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 59f10f18f72111093e0c97906cde883ede6795065350984f0a12910f9fc99b73
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57218566"
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