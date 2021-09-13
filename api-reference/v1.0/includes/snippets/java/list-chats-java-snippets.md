---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5c99527b46300a81b702fe17e266b2364b6e33c6
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59038321"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ChatCollectionPage chats = graphClient.users("8b081ef6-4792-4def-b2c9-c363a1bf41d5").chats()
    .buildRequest()
    .get();

```