---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 89a420eafb41f8a2fd5dcd0c2fcc1603f5b1370c
ms.sourcegitcommit: fe1b4d098af604cc34596f595e799911ea672532
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/07/2021
ms.locfileid: "51611646"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ChatMessage chatMessage = graphClient.teams("fbe2bf47-16c8-47cf-b4a5-4b9b187c508b").channels("19:4a95f7d8db4c4e7fae857bcebe0623e6@thread.tacv2").messages("1614618259349")
    .buildRequest()
    .get();

```