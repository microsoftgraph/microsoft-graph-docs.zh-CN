---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d83ae0fd5557cc9b0f39872f62feb6a0dba59b59
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48981307"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String message = "Approved!";

graphClient.teams("{teamId}").schedule().offerShiftRequests("{offerShiftRequestId}")
    .approve(message)
    .buildRequest()
    .post();

```