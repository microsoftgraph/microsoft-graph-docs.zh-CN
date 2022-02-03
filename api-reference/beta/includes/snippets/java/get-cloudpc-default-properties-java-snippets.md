---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0d33c8c78e7df885c30e72da3261153248b5cf38
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62341230"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

CloudPC cloudPC = graphClient.deviceManagement().virtualEndpoint().cloudPCs("9ec90ff8-fd63-4fb9-ab5a-aa4fdcc43ec9")
    .buildRequest()
    .get();

```