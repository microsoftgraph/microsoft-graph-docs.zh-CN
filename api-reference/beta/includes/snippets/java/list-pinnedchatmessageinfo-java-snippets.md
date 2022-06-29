---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d460d8571e151d87fbd01c7ed4f2e38743a48b7b
ms.sourcegitcommit: 54ba08a80db85b9e84813387e8c4416eca44fa8e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/26/2022
ms.locfileid: "65695001"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PinnedChatMessageInfoCollectionPage pinnedMessages = graphClient.chats("19:d65713bc498c4a428c71ef9353e6ce20@thread.v2").pinnedMessages()
    .buildRequest()
    .expand("message")
    .get();

```