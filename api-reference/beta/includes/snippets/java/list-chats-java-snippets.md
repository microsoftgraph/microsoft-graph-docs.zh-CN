---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 92b9f74f923bc317f174d67dd5028544995a7008b2a22426be8f30f0dae9447a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57106369"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ChatCollectionPage chats = graphClient.users("8b081ef6-4792-4def-b2c9-c363a1bf41d5").chats()
    .buildRequest()
    .get();

```