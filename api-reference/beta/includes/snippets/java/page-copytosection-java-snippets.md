---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0fd34a9f7cdfa424b089b98dc79ddf39e0a6c431
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48964407"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String id = "id-value";

String groupId = "groupId-value";

graphClient.me().onenote().pages("{id}")
    .copyToSection(id,groupId,null,null)
    .buildRequest()
    .post();

```