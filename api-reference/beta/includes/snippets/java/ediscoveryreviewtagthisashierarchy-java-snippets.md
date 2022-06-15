---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7929dddf9de50d36c58213fcbf72474181e3961e
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2022
ms.locfileid: "66094808"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EdiscoveryReviewTagAsHierarchyCollectionPage asHierarchy = graphClient.security().cases().ediscoveryCases("58399dff-cebe-478f-b1af-d3227f1fd645").tags()
    .asHierarchy()
    .buildRequest()
    .get();

```