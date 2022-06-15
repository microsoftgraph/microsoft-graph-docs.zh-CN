---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2ecb081bf00d41bd88722c1c2707e9ff115e2269
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2022
ms.locfileid: "66093880"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EdiscoveryReviewSetQueryRunCollectionPage run = graphClient.security().cases().ediscoveryCases("58399dff-cebe-478f-b1af-d3227f1fd645").reviewSets("273f11a1-17aa-419c-981d-ff10d33e420f").queries("837335b0-1943-444d-a3d1-5522cc21c5a4")
    .run()
    .buildRequest()
    .get();

```