---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7ebc8e3138ae22b342d6706867f5461cb7555d5e
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/30/2021
ms.locfileid: "53210255"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var teamworkTag = await graphClient.Teams["{team-id}"].Tags["{teamworkTag-id}"]
    .Request()
    .GetAsync();

```