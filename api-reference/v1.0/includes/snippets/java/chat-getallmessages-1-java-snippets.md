---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 320b19d2b8befc360ae2b489e0b46cec1ed215a3
ms.sourcegitcommit: 2a9b82dae63d8a998711679a379ae1fa89df80e0
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/06/2021
ms.locfileid: "60214481"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ChatGetAllMessagesCollectionPage getAllMessages = graphClient.users("0b4f1cf6-54c8-4820-bbb7-2a1f4257ade5").chats()
    .getAllMessages()
    .buildRequest()
    .top(2)
    .get();

```