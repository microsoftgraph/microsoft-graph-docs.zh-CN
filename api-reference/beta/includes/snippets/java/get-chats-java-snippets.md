---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 29ab3c17d304c5135e36ba7bdef1a19d0568218f
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35863630"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IChatCollectionPage chats = graphClient.users("{id}").chats()
    .buildRequest()
    .get();

```