---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ba22af5542a86660204722bbd6ace7b4a86c8837
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50443306"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var userAccountInformation = await graphClient.Me.Profile.Account["{id}"]
    .Request()
    .GetAsync();

```