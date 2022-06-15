---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d7028bb86c20fb4925e10aa67729788f3180b1e1
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2022
ms.locfileid: "66096165"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EdiscoveryCase ediscoveryCase = graphClient.security().cases().ediscoveryCases("22aa2acd-7554-4330-9ba9-ce20014aaae4")
    .buildRequest()
    .get();

```