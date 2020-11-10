---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 09b3771037fb7520c7d5c2eaa8e5f43e2a287a19
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48968594"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Calendar calendar = new Calendar();
calendar.name = "Volunteer";

graphClient.me().calendars()
    .buildRequest()
    .post(calendar);

```