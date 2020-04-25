---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 01c3a5689e91bdf64934fd6f3a5b03a98cdf65da
ms.sourcegitcommit: 5575e6607817ba23ceb0b01e2f5fc81e58bdcd1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/22/2020
ms.locfileid: "43806594"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

CalendarPermission calendarPermission = graphClient.users("{id}").calendar().calendarPermissions("{id}")
    .buildRequest()
    .get();

```