---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7be05ffd1451446b5ecb56e921b4bf49e81f0f18
ms.sourcegitcommit: c650b95ef4d0c3e93e2eb36cd6b52ed31200164f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/10/2020
ms.locfileid: "44683762"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var users = await graphClient.Users
    .Request()
    .Filter("startswith(displayName,'Eric'),")
    .Select("displayName,signInActivity")
    .GetAsync();

```