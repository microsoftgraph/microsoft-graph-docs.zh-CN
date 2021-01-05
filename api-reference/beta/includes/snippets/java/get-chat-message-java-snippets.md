---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5a326f6118e1e07e708550b17bd2bd9750e2b815
ms.sourcegitcommit: a1675c7b8dfc7d7c3c7923d06cda2b0127f9c3e6
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/05/2021
ms.locfileid: "49756016"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ChatMessage chatMessage = graphClient.me().chats("{id}").messages("{id}")
    .buildRequest()
    .get();

```