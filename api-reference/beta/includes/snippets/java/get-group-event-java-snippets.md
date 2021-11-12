---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 42a3a7b5ac9b4cda3671dc580d29e653f8ad97ee2011fb69b8eecfee14f03ba6
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57161554"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Event event = graphClient.groups("02bd9fd6-8f93-4758-87c3-1fb73740a315").events("AQMkAGI5MWY5ZmUyLTJiNzYtNDE0ZC04OWEwLWM3M2FjYmM3NwAzZWYARgAAA_b2VnUAiWNLj0xeSOs499YHAMT2RdsuOqRIlQZ4vOzp66YAAAIBDQAAAMT2RdsuOqRIlQZ4vOzp66YAAAIJOgAAAA==")
    .buildRequest()
    .get();

```