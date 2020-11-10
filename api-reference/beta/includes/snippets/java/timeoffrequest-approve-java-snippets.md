---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 16a27b3d813f925f5493abe02e1a43d2fbbf43af
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48981370"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String message = "message-value";

graphClient.teams("{teamId}").schedule().timeOffRequests("{timeOffRequestId}")
    .approve(message)
    .buildRequest()
    .post();

```