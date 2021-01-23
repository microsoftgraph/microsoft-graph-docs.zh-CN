---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 80750f25a502310e9a17d20e9bf881491a667262
ms.sourcegitcommit: 9a5facff47a8d4e05ecd2c6cd68294a948c47c4d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2021
ms.locfileid: "49946310"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

UserScopeTeamsAppInstallation userScopeTeamsAppInstallation = graphClient.users("{id}").teamwork().installedApps("{id}")
    .buildRequest()
    .get();

```