---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0d3e239eaa45df323ca1d2f3630b6eb6fb55d313
ms.sourcegitcommit: 48fff935d56fe96e97577a80a3a0aa15c45419ba
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/10/2021
ms.locfileid: "50179270"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var users = await graphClient.Users
    .Request()
    .Filter("startswith(displayName,'Eric')")
    .Select("displayName,signInActivity")
    .GetAsync();

```