---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: aea1f1e15ac659b3c29fcdd768e95c4f87e2a5b1
ms.sourcegitcommit: 60ced1be6ed8dd2d23263090a1cfbc16689bb043
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/28/2020
ms.locfileid: "48782989"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Content members = graphClient.me().chats().{id}().members()
    .buildRequest()
    .get();

```