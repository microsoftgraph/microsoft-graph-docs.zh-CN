---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 68e7060cbe8d75a11b2e311a82d0315c35184d9b
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50787653"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var userAccountInformation = await graphClient.Me.Profile.Account["{userAccountInformation-id}"]
    .Request()
    .GetAsync();

```