---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 55c51eb35ad43670c1e68c72423cf6dbd0b18613
ms.sourcegitcommit: 75428fc7535662f34e965c6b69fef3a53fdaf1cb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/16/2020
ms.locfileid: "49689306"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var teamsApps = await graphClient.AppCatalogs.TeamsApps
    .Request()
    .Filter("id eq 'b1c5353a-7aca-41b3-830f-27d5218fe0e5'")
    .GetAsync();

```