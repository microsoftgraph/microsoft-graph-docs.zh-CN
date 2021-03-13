---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4de4455e198fe9fc51c78078ff5eaa51ef42ca8f
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50790563"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var personAward = await graphClient.Me.Profile.Awards["{personAward-id}"]
    .Request()
    .GetAsync();

```