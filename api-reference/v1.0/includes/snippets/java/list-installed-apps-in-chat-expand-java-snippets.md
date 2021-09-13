---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d021783cb74f88d2a588d1ab28ceaaff85057d29bb336bee988f7a91eee94342
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57106826"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

TeamsAppInstallationCollectionPage installedApps = graphClient.chats("19:d65713bc498c4a428c71ef9353e6ce20@thread.v2").installedApps()
    .buildRequest()
    .expand("teamsAppDefinition($expand=bot)")
    .get();

```