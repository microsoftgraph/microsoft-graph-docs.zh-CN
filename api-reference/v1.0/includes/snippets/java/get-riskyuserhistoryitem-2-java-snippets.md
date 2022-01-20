---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 95f29a82d444909057192fff9664b19dae2c84a0
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62091853"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

RiskyUserHistoryItemCollectionPage history = graphClient.identityProtection().riskyUsers("{riskyUserId}").history()
    .buildRequest()
    .get();

```