---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 94354278a82fe28c1c35566dda4cf9163a153a02
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2022
ms.locfileid: "66093693"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EdiscoveryReviewTag ediscoveryReviewTag = new EdiscoveryReviewTag();
ediscoveryReviewTag.displayName = "My tag API 2";
ediscoveryReviewTag.description = "Use Graph API to create tags (updated)";

graphClient.security().cases().ediscoveryCases("58399dff-cebe-478f-b1af-d3227f1fd645").tags("062de822f17a4a2e9b833aa3f6c37108")
    .buildRequest()
    .patch(ediscoveryReviewTag);

```