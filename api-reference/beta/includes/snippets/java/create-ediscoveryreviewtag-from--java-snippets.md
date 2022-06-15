---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 903f2ffa2c6b75f10399f1cdcef88fe270488ad8
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2022
ms.locfileid: "66092143"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EdiscoveryReviewTagCollectionPage tags = graphClient.security().cases().ediscoveryCases("58399dff-cebe-478f-b1af-d3227f1fd645").tags()
    .buildRequest()
    .get();

```