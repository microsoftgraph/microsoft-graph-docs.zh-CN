---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 55c51eb35ad43670c1e68c72423cf6dbd0b18613
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/19/2020
ms.locfileid: "46806283"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var teamsApps = await graphClient.AppCatalogs.TeamsApps
    .Request()
    .Filter("id eq 'b1c5353a-7aca-41b3-830f-27d5218fe0e5'")
    .GetAsync();

```