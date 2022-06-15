---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a669b3dbbc3e209733448a1fff810a3f83a6b83f
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2022
ms.locfileid: "66094683"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EdiscoveryReviewSetQuery ediscoveryReviewSetQuery = new EdiscoveryReviewSetQuery();
ediscoveryReviewSetQuery.displayName = "My Query 1";
ediscoveryReviewSetQuery.contentQuery = "(Author=\"edison\")";

graphClient.security().cases().ediscoveryCases("58399dff-cebe-478f-b1af-d3227f1fd645").reviewSets("273f11a1-17aa-419c-981d-ff10d33e420f").queries()
    .buildRequest()
    .post(ediscoveryReviewSetQuery);

```