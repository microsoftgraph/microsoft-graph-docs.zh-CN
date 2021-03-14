---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2f81f811be6f1cb3466b4355e55c1fc5abff5e1b
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50798858"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var installedApps = await graphClient.Teams["{team-id}"].InstalledApps
    .Request()
    .Expand("teamsAppDefinition")
    .GetAsync();

```