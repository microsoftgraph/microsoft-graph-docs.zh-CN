---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 313b8cc4790797589d51dff950ce002daa503ac5bd1d94d71b7aeb48a1a8d144
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57218514"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ChatMessageCollectionPage replies = graphClient.teams("fbe2bf47-16c8-47cf-b4a5-4b9b187c508b").channels("19:4a95f7d8db4c4e7fae857bcebe0623e6@thread.tacv2").messages("1616989510408").replies()
    .buildRequest()
    .get();

```