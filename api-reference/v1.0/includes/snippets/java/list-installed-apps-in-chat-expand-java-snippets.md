---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 22dfe02b6b684e4ed4a04acb032aa56443e88f1f
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50958497"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

TeamsAppInstallationCollectionPage installedApps = graphClient.chats("19:d65713bc498c4a428c71ef9353e6ce20@thread.v2").installedApps()
    .buildRequest()
    .expand("teamsAppDefinition($expand=bot)")
    .get();

```