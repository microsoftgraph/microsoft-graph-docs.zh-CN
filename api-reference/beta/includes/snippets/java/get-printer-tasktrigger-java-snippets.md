---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5d593d27ec026c5a0a24891c4748b08943f159952f3be5f40c7b849e5df0d84a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57163652"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PrintTaskTrigger printTaskTrigger = graphClient.print().printers("{printerId}").taskTriggers("{taskTriggerId}")
    .buildRequest()
    .get();

```