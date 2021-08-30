---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 29b62570ce67f7aab0c6d62dcc5a89c062f89e67eaa3bd37330bde224eb388ac
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57162827"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Chat chat = graphClient.chats("19:b8577894a63548969c5c92bb9c80c5e1@thread.v2")
    .buildRequest()
    .expand("members")
    .get();

```