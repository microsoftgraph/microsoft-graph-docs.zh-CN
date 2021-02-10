---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 85784740fa92cf84d95ca37bc91c7c8a8ed389cc
ms.sourcegitcommit: 48fff935d56fe96e97577a80a3a0aa15c45419ba
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/10/2021
ms.locfileid: "50179366"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var teamsApps = await graphClient.AppCatalogs.TeamsApps
    .Request()
    .Filter("id eq '876df28f-2e78-423b-94a5-44181bd0e225'")
    .Expand("appDefinitions")
    .GetAsync();

```