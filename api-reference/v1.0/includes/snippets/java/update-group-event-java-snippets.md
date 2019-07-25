---
description: 自动生成的文件。 不修改
ms.openlocfilehash: eb19b2be62988db1e7f08e4dea8d1e0ed42a928c
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35885346"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Event event = new Event();
Location location = new Location();
location.displayName = "Conf Room 2";
event.location = location;

graphClient.groups("01d4ee64-15ce-491e-bad1-b91aa3223df4").calendar().events("AAMkADZlAAAAABERAAA=")
    .buildRequest()
    .patch(event);

```