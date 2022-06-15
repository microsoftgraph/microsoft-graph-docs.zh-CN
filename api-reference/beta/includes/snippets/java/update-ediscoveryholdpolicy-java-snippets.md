---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5ef72d076d7d53d177855372264b7d23e824909d
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2022
ms.locfileid: "66093925"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EdiscoveryHoldPolicy ediscoveryHoldPolicy = new EdiscoveryHoldPolicy();
ediscoveryHoldPolicy.description = "updated description";
ediscoveryHoldPolicy.contentQuery = "bazooka bazooka";

graphClient.security().cases().ediscoveryCases("b0073e4e-4184-41c6-9eb7-8c8cc3e2288b").legalHolds("783c3ea4-d474-4051-9c13-08707ce8c8b6")
    .buildRequest()
    .patch(ediscoveryHoldPolicy);

```