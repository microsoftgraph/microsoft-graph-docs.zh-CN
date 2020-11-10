---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: aa1a187fa52db8b23f162de729656ed92abcb6ac
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48978681"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String id = "id-value";

String groupId = "groupId-value";

String renameAs = "renameAs-value";

graphClient.me().onenote().sections("{id}")
    .copyToNotebook(id,groupId,renameAs,null,null)
    .buildRequest()
    .post();

```