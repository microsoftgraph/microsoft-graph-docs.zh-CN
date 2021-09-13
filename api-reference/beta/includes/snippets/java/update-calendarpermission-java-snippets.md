---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 62aa2c3419d039b210d3790a33bd000ea2107f3322c9c9f1b5d46bd77664267d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57218602"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

CalendarPermission calendarPermission = new CalendarPermission();
calendarPermission.role = CalendarRoleType.WRITE;

graphClient.users("{id}").calendar().calendarPermissions("RGVmYXVsdA==")
    .buildRequest()
    .patch(calendarPermission);

```