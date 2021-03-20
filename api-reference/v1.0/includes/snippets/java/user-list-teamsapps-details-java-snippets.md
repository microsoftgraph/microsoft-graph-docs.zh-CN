---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5ec8ec4b463c37a1cf66477411d6254b3e648c2e
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50956102"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

UserScopeTeamsAppInstallationCollectionPage installedApps = graphClient.users("5b649834-7412-4cce-9e69-176e95a394f5").teamwork().installedApps()
    .buildRequest()
    .expand("teamsAppDefinition")
    .get();

```