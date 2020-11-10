---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 466784902ccd543ed0e65d0b19921ed8be280ecc
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48976799"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String message = "message-value";

graphClient.teams("{teamId}").schedule().swapShiftsChangeRequests("{swapShiftChangeRequestId}")
    .decline(message)
    .buildRequest()
    .post();

```