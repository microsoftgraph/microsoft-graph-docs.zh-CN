---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 01c205026181f3ba283f4410693dacd2617e9b10
ms.sourcegitcommit: 2a35434fabc76672e21bfc3ed5a1d28f9f3b66bc
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2021
ms.locfileid: "52254219"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Chat chat = graphClient.users("8b081ef6-4792-4def-b2c9-c363a1bf41d5").chats("19:8b081ef6-4792-4def-b2c9-c363a1bf41d5_877192bd-9183-47d3-a74c-8aa0426716cf@unq.gbl.spaces")
    .buildRequest()
    .get();

```