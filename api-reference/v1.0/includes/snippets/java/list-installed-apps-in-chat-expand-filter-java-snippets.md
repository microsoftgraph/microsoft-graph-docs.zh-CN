---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 820c879109f6d167740e0fa790f0cfabea0053a0
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2022
ms.locfileid: "63351228"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

TeamsAppInstallationCollectionPage installedApps = graphClient.chats("19:d65713bc498c4a428c71ef9353e6ce20@thread.v2").installedApps()
    .buildRequest()
    .filter("teamsApp/externalId eq 'cf1ba4c7-f94e-4d80-ba90-5594b641a8ee'")
    .expand("teamsApp,teamsAppDefinition")
    .get();

```