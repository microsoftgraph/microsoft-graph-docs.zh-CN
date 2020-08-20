---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 84d0cf5507b3c61e3aa4a2f1831d2fe92683de09
ms.sourcegitcommit: 239db9e961e42b505f52de9859963a9136935f2f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/20/2020
ms.locfileid: "46819955"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var publications = await graphClient.Me.Profile.Publications
    .Request()
    .GetAsync();

```