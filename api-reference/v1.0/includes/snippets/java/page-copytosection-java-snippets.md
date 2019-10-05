---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 0fd34a9f7cdfa424b089b98dc79ddf39e0a6c431
ms.sourcegitcommit: 46ee19b244349e2a1537f0c44c576d7c01cf03a9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/05/2019
ms.locfileid: "37402753"
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