---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6813a3fc91cc93654e99507e3dee1c0bb6f7b1a3
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2022
ms.locfileid: "66092949"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EdiscoveryHoldPolicy ediscoveryHoldPolicy = graphClient.security().cases().ediscoveryCases("b0073e4e-4184-41c6-9eb7-8c8cc3e2288b").legalHolds("783c3ea4-d474-4051-9c13-08707ce8c8b6")
    .buildRequest()
    .get();

```