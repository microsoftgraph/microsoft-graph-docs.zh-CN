---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6124113641c908b9ff9f5fd5929bcf45628f3f48
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2022
ms.locfileid: "66095434"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EdiscoveryReviewSetQuery ediscoveryReviewSetQuery = graphClient.security().cases().ediscoveryCases("58399dff-cebe-478f-b1af-d3227f1fd645").reviewSets("273f11a1-17aa-419c-981d-ff10d33e420f").queries("fcb86cd1-50e0-427c-840e-ba6f087364e5")
    .buildRequest()
    .get();

```