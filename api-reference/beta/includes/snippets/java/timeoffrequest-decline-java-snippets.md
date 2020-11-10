---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 33f5973c4041b5a0a2bf267167e7dff6032318be
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48981356"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String message = "message-value";

graphClient.teams("{teamId}").schedule().timeOffRequests("{timeOffRequestId}")
    .decline(message)
    .buildRequest()
    .post();

```