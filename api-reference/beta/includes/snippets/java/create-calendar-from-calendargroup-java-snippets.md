---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4921e2395b03e0dfccf292ee4129cc454de05ddb90410fcd6477bf7439c6057f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57162935"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Calendar calendar = new Calendar();
calendar.name = "Marketing calendar";

graphClient.me().calendarGroups("AAMkADYAAAR9NR5AAA=").calendars()
    .buildRequest()
    .post(calendar);

```