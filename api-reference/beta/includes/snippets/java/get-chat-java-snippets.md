---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 01c205026181f3ba283f4410693dacd2617e9b10
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50980220"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Chat chat = graphClient.users("8b081ef6-4792-4def-b2c9-c363a1bf41d5").chats("19:8b081ef6-4792-4def-b2c9-c363a1bf41d5_877192bd-9183-47d3-a74c-8aa0426716cf@unq.gbl.spaces")
    .buildRequest()
    .get();

```