---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0e8af67d340bb6dded2cea659d4f65cc2b34356cf2a8f5205d565d2ffc07e092
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57218608"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

CalendarPermission calendarPermission = graphClient.users("{id}").calendar().calendarPermissions("{id}")
    .buildRequest()
    .get();

```