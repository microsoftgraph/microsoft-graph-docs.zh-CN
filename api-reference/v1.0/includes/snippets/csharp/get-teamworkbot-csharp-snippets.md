---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: cfbd90ee84d1ea2c75b503794c011fd9f7696bb3
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50774755"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var teamworkBot = await graphClient.AppCatalogs.TeamsApps["{teamsApp-id}"].AppDefinitions["{teamsAppDefinition-id}"].Bot
    .Request()
    .GetAsync();

```