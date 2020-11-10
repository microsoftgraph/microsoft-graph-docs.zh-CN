---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c12e1cc0b2cff9ed3e8976fe82f09b552607644c
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48968300"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.print().printers("{id}").jobs("{id}")
    .cancel()
    .buildRequest()
    .post();

```