---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8209fb9af288ef9f63c2d5fef78dbf16a012f259
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50969505"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ConversationMember conversationMember = graphClient.chats("19:cf66807577b149cca1b7af0c32eec122@thread.v2").members("141c574c-dd90-4131-b173-baf4bb0e894e")
    .buildRequest()
    .get();

```