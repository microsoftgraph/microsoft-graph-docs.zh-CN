---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9a209dac6165eadd4678d5219224c2686b1edb80
ms.sourcegitcommit: 239db9e961e42b505f52de9859963a9136935f2f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/20/2020
ms.locfileid: "46819632"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var personInterest = await graphClient.Me.Profile.Interests["{id}"]
    .Request()
    .GetAsync();

```