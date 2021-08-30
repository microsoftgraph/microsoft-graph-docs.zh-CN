---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 20c3373accc56985d82010e3b87731d0500c50c43b18cc76d4a9d25a0153d300
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57278801"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

TeamsAppInstallationCollectionPage installedApps = graphClient.chats("19:d65713bc498c4a428c71ef9353e6ce20@thread.v2").installedApps()
    .buildRequest()
    .get();

```