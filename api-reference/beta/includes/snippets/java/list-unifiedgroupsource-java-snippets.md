---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2e8812d57f5010b9eff5741bf19a8b5617f5c4c6
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2022
ms.locfileid: "66094962"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

UnifiedGroupSourceCollectionPage unifiedGroupSources = graphClient.security().cases().ediscoveryCases("b0073e4e-4184-41c6-9eb7-8c8cc3e2288b").custodians("0053a61a3b6c42738f7606791716a22a").unifiedGroupSources()
    .buildRequest()
    .get();

```