---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7b86ded7b325cf7a7b4a472e719f89be56f4f87b
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2022
ms.locfileid: "66096278"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EdiscoveryHoldPolicyCollectionPage legalHolds = graphClient.security().cases().ediscoveryCases("b0073e4e-4184-41c6-9eb7-8c8cc3e2288b").legalHolds()
    .buildRequest()
    .get();

```