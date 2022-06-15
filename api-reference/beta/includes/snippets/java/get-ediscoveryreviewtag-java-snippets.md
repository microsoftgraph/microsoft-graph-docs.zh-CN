---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3e74dfe91ffd1f1a625865f0f5ff8e5de56cf9d3
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2022
ms.locfileid: "66094332"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EdiscoveryReviewTag ediscoveryReviewTag = graphClient.security().cases().ediscoveryCases("58399dff-cebe-478f-b1af-d3227f1fd645").tags("062de822f17a4a2e9b833aa3f6c37108")
    .buildRequest()
    .get();

```