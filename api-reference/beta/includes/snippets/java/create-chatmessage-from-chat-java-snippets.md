---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 5cf64963c3063896ff1fe317402cdbbf8e36b9b1
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35863645"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ChatMessage chatMessage = new ChatMessage();
ItemBody body = new ItemBody();
body.content = "Hello world";
chatMessage.body = body;

graphClient.teams("{id}").channels("{id}").messages()
    .buildRequest()
    .post(chatMessage);

```