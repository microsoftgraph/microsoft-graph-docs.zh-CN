---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3ccf585e5a8bfb9968a5de13b5d244fc5b76c6e5
ms.sourcegitcommit: 82da4012294b046416c9ae93d2294d80dab217f6
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/04/2020
ms.locfileid: "48905685"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var users = await graphClient.Users
    .Request()
    .Select("displayName,userPrincipalName,signInActivity")
    .GetAsync();

```