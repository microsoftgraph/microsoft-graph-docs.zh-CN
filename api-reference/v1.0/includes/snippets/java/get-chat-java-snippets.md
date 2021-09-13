---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 67d965f68b0401425ccbd2daa89bdd779665b8468e1a82bbc0a6dabe93a99958
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57104336"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Chat chat = graphClient.users("8b081ef6-4792-4def-b2c9-c363a1bf41d5").chats("19:8b081ef6-4792-4def-b2c9-c363a1bf41d5_877192bd-9183-47d3-a74c-8aa0426716cf@unq.gbl.spaces")
    .buildRequest()
    .get();

```