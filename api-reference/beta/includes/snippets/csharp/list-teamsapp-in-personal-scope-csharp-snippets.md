---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e1a8e9ef5adcf25bbc06b7515021621b6d1fa5ea
ms.sourcegitcommit: 412507a3c3a8e407fcc43b7cd227d4db35791f58
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2021
ms.locfileid: "51765964"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var teamsApps = await graphClient.AppCatalogs.TeamsApps
    .Request()
    .Filter("appDefinitions/any(a:a/allowedInstallationScopes has 'personal')")
    .Expand("appDefinitions($select=id,displayName,allowedInstallationScopes)")
    .GetAsync();

```