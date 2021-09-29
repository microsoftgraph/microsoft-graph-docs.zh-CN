---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 23c50bea314faddbe8e304393f5a408562b0ab79
ms.sourcegitcommit: 36bae3615df41876493b25da478e589d1974f97b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/29/2021
ms.locfileid: "59996210"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

CalendarPermission calendarPermission = new CalendarPermission();
EmailAddress emailAddress = new EmailAddress();
emailAddress.name = "Samantha Booth";
emailAddress.address = "samanthab@adatum.onmicrosoft.com";
calendarPermission.emailAddress = emailAddress;
calendarPermission.isInsideOrganization = true;
calendarPermission.isRemovable = true;
calendarPermission.role = CalendarRoleType.READ;

graphClient.me().calendar().calendarPermissions()
    .buildRequest()
    .post(calendarPermission);

```