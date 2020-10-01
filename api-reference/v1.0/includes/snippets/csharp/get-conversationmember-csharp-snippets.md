---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0f5ac7ae03d2b92ec69e3a7d417c4d28af810d41
ms.sourcegitcommit: a9f0fde9924ad184d315bb2de43c2610002409f3
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/30/2020
ms.locfileid: "48314502"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var members = await graphClient.Teams["{teamsId}"].Members
    .Request()
    .GetAsync();

```