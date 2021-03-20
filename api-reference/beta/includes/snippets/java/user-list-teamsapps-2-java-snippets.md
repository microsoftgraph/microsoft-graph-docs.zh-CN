---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 11294fa34f1bf0f1404cee38ddbbed69f91a6f84
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50941976"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IUserScopeTeamsAppInstallationCollectionPage installedApps = graphClient.users("{id}").teamwork().installedApps()
    .buildRequest()
    .get();

```