---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 964556822075a4b075a4d1dd484c1c0b8bce2821
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48981842"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkPosition workPosition = new WorkPosition();
workPosition.isCurrent = true;

graphClient.me().profile().positions("{id}")
    .buildRequest()
    .patch(workPosition);

```