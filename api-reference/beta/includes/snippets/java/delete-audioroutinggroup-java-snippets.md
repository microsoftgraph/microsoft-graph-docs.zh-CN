---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c35d2f33ebf99b632d8eb170a26b91720e0b1297
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48961609"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.communications().calls("{id}").audioRoutingGroups("{id}")
    .buildRequest()
    .delete();

```