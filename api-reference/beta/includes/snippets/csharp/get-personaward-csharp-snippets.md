---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 421f8c833af5cd0894f592c59046eeb61a2e563b
ms.sourcegitcommit: 239db9e961e42b505f52de9859963a9136935f2f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/20/2020
ms.locfileid: "46820164"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var personAward = await graphClient.Me.Profile.Awards["{id}"]
    .Request()
    .GetAsync();

```