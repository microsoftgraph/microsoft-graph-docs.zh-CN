---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9c8861f6005580a1d9866ea6dfc6e70bf24478a6
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50958274"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Chat chat = new Chat();
chat.topic = "Group chat title update";

graphClient.chats("19:1c5b01696d2e4a179c292bc9cf04e63b@thread.v2")
    .buildRequest()
    .patch(chat);

```