---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7878dd907b92a147a970170c3e5e8167e58013c0
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/30/2021
ms.locfileid: "53210261"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

TeamsAsyncOperation teamsAsyncOperation = graphClient.chats("19:c253a29b5f694b55a6baad8e83510af7@thread.v2").operations("2432b57b-0abd-43db-aa7b-16eadd115d34-e88ae9aa-887e-4972-ac3e-bd578e38232e-cf58835e-43f0-4fc1-825e-5de55630e7e4")
    .buildRequest()
    .get();

```