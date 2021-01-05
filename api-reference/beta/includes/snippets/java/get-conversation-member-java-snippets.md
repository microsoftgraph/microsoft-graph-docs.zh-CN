---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0e3cac8ed6783e6a47d4ab74ab607b49aaca0425
ms.sourcegitcommit: a1675c7b8dfc7d7c3c7923d06cda2b0127f9c3e6
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/05/2021
ms.locfileid: "49753715"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ConversationMember conversationMember = graphClient.chats("19:cf66807577b149cca1b7af0c32eec122@thread.v2").members("141c574c-dd90-4131-b173-baf4bb0e894e")
    .buildRequest()
    .get();

```