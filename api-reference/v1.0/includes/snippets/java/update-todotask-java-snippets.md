---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4b1e068ad2c1150e8326a30d30f298735f800da9
ms.sourcegitcommit: 82da4012294b046416c9ae93d2294d80dab217f6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/04/2020
ms.locfileid: "48905324"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

TodoTask todoTask = new TodoTask();
DateTimeTimeZone dueDateTime = new DateTimeTimeZone();
dueDateTime.dateTime = "2020-07-25T16:00:00";
dueDateTime.timeZone = "Eastern Standard Time";
todoTask.dueDateTime = dueDateTime;

graphClient.me().todo().lists("AAMkADA1MTHgwAAA=").tasks("721a35e2-35e2-721a-e235-1a72e2351a72")
    .buildRequest()
    .patch(todoTask);

```