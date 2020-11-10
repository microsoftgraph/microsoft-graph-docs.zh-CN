---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c5cc2fb7d41ccaba17d76ae012d6dd9fdc83f63e
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48951500"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String groupId = "groupId-value";

String renameAs = "renameAs-value";

graphClient.me().onenote().notebooks("{id}")
    .copyNotebook(groupId,renameAs,null,null,null)
    .buildRequest()
    .post();

```