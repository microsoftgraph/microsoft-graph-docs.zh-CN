---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 512e6bd147e311d57d60b1bbfd41188b2fd1526e
ms.sourcegitcommit: e497ed9bb56400bdd2bb53d52ddf057d9966220b
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/30/2021
ms.locfileid: "61226630"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

User user = graphClient.users("{id}")
    .buildRequest()
    .select("customSecurityAttributes")
    .get();

```