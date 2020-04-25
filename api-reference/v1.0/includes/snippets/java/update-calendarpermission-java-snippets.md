---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 671f9387162498ed233ab8c5b1821f4817076928
ms.sourcegitcommit: 5575e6607817ba23ceb0b01e2f5fc81e58bdcd1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/22/2020
ms.locfileid: "43806556"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

CalendarPermission calendarPermission = new CalendarPermission();
calendarPermission.role = CalendarRoleType.WRITE;

graphClient.users("{id}").calendar().calendarPermissions("RGVmYXVsdA==")
    .buildRequest()
    .patch(calendarPermission);

```