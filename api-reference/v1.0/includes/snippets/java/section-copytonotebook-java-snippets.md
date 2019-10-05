---
description: 自动生成的文件。 不修改
ms.openlocfilehash: aa1a187fa52db8b23f162de729656ed92abcb6ac
ms.sourcegitcommit: 46ee19b244349e2a1537f0c44c576d7c01cf03a9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/05/2019
ms.locfileid: "37402739"
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