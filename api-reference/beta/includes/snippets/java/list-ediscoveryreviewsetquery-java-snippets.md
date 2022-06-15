---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 52dd195b3f6cd604cf4ec6d87f76f8421e0e7612
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2022
ms.locfileid: "66095438"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EdiscoveryReviewSetQueryCollectionPage queries = graphClient.security().cases().ediscoveryCases("58399dff-cebe-478f-b1af-d3227f1fd645").reviewSets("273f11a1-17aa-419c-981d-ff10d33e420f").queries()
    .buildRequest()
    .get();

```