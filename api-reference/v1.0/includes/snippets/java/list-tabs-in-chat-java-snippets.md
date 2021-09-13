---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9dc5d858e8bdd8f1b18ed8b0a4d8b25a6e296df521a1654446eb0646c146a579
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56904159"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

TeamsTabCollectionPage tabs = graphClient.chats("19:d65713bc498c4a428c71ef9353e6ce20@thread.v2").tabs()
    .buildRequest()
    .expand("teamsApp")
    .get();

```