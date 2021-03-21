---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 88236c6a7006d9c8ca780491d8d240a69812beed
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50980147"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PrintTaskTrigger printTaskTrigger = graphClient.print().printers("{printerId}").taskTriggers("{printTaskTriggerId}")
    .buildRequest()
    .get();

```