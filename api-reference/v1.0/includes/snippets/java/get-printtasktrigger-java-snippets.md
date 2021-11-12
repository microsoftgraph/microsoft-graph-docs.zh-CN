---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2c9c32af35ca1ec57ab6ccd53c864637d0d530efeefdea1ac5fbf81fb02d9af7
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57162546"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PrintTaskTrigger printTaskTrigger = graphClient.print().printers("{printerId}").taskTriggers("{printTaskTriggerId}")
    .buildRequest()
    .get();

```