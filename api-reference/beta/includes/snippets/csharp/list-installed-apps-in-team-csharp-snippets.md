---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 431e3983d67216552d86ebf13ab4aee87aa0c9c0
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50788710"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var installedApps = await graphClient.Teams["{team-id}"].InstalledApps
    .Request()
    .GetAsync();

```