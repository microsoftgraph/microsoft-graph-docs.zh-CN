---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 072ab1873b6f3538d6c4807e80e88e8c16685cafcdd4597e080fd4f9a128775e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57103934"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Schedule schedule = new Schedule();
schedule.enabled = true;
schedule.timeZone = "America/Chicago";

graphClient.teams("{teamId}").schedule()
    .buildRequest()
    .put(schedule);

```