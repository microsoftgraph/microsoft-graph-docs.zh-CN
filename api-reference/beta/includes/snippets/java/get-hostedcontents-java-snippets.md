---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8fd5bdf2e1e25a1cc2d31835a424798bccbaa85f
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48958184"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IChatMessageHostedContentCollectionPage hostedContents = graphClient.chats("{id}").messages("{id}").hostedContents()
    .buildRequest()
    .get();

```