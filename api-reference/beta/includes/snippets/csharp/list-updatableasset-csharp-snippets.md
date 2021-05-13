---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b90332d6a081be6e5e333d199898d1a53174c83c
ms.sourcegitcommit: b8b0e88b3ba9a434dc45f5ab640cb46f66fae299
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/13/2021
ms.locfileid: "52476787"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var exclusions = await graphClient.Admin.Windows.Updates.Deployments["{windowsUpdates.deployment-id}"].Audience.Exclusions
    .Request()
    .GetAsync();

```