---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e1b3b2461d636e2fe428da3589c5df8402c2e7a0
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50798943"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IConversationMemberCollectionPage members = graphClient.chats("{id}").members()
    .buildRequest()
    .get();

```