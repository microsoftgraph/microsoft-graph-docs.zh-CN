---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0c959d000ddbef0834fdc75b09212bbf6fa05ddb
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48979143"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Schedule schedule = graphClient.teams("{teamId}").schedule()
    .buildRequest()
    .get();

```