---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d0c7f967197b4ea2f6f07de3d9caf22ed09817aed992e421460426b4d96d8ad6
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57332700"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ConversationThread conversationThread = graphClient.groups("{id}").threads("{id}")
    .buildRequest()
    .get();

```