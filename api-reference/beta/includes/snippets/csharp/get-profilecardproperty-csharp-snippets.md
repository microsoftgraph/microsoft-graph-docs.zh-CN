---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 434c291c87b0dc7548f591bb5cae5a521b6dc19f
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50810291"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var profileCardProperty = await graphClient.Organization["{organization-id}"].Settings.ProfileCardProperties["{profileCardProperty-id}"]
    .Request()
    .GetAsync();

```