---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ce5a7cb615ff6af484a938372136e32cc1a94b84
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50798194"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var presence = await graphClient.Users["{user-id}"].Presence
    .Request()
    .GetAsync();

```