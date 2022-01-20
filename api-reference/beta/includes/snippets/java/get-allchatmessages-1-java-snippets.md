---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 264740dc4d1882b25106ae92bd461871e2b7b43b
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62100541"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ChatMessageCollectionPage messages = graphClient.chats("19:2da4c29f6d7041eca70b638b43d45437@thread.v2").messages()
    .buildRequest()
    .orderBy("createdDateTime")
    .top(2)
    .get();

```