---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e9e3ad1968c0f6e935aff24afc8c569a8721e4e2
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50956101"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

UserScopeTeamsAppInstallationCollectionPage installedApps = graphClient.users("97a5a533-833d-494b-b543-c0afe026cb96").teamwork().installedApps()
    .buildRequest()
    .filter("teamsApp/externalId eq 'cf1ba4c7-f94e-4d80-ba90-5594b641a8ee'")
    .expand("teamsAppDefinition")
    .get();

```