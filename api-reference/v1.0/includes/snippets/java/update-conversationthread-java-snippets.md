---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4a435fd0e999d82a694caf4ac0ae0ecc029de84dd71872de7639ac4f41166d9d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57333542"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ConversationThread conversationThread = new ConversationThread();
conversationThread.isLocked = true;

graphClient.groups("{id}").threads("{id}")
    .buildRequest()
    .patch(conversationThread);

```