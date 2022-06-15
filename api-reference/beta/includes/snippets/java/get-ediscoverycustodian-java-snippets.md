---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b778d1a9fff1d7c2215299b0d3e88922ff2a48d1
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2022
ms.locfileid: "66095837"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EdiscoveryCustodian ediscoveryCustodian = graphClient.security().cases().ediscoveryCases("b0073e4e-4184-41c6-9eb7-8c8cc3e2288b").custodians("0053a61a3b6c42738f7606791716a22a")
    .buildRequest()
    .get();

```