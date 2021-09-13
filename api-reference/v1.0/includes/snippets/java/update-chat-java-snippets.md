---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9c054d31e0422537279ff3b6022ab31c80095955bec32fdaa628b797643c3956
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56904149"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Chat chat = new Chat();
chat.topic = "Group chat title update";

graphClient.chats("19:1c5b01696d2e4a179c292bc9cf04e63b@thread.v2")
    .buildRequest()
    .patch(chat);

```