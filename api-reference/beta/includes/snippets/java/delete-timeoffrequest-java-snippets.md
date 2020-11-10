---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: cf81e0dcd7eb8788e74a2696524a6c20a2fee69e
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48981341"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.teams("{teamId}").schedule().timeOffRequests("{timeOffRequestId}")
    .buildRequest()
    .delete();

```