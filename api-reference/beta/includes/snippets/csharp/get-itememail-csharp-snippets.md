---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bb9afe5ef269420a3dfe455490ea2598d8e50384
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50797611"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var itemEmail = await graphClient.Users["{user-id}"].Profile.Emails["{itemEmail-id}"]
    .Request()
    .GetAsync();

```