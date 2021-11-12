---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 88465c8ad74a9bec4c822228b966b310528b35cfbe3d519b722f529ae4aeef8c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57409691"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.print().printers("{printerId}").taskTriggers("{printTaskTriggerId}")
    .buildRequest()
    .delete();

```