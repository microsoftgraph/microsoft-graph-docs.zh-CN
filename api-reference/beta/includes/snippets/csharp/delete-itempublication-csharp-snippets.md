---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 873fe152ea0de44bfcee5af3a07524342a2a3354
ms.sourcegitcommit: 239db9e961e42b505f52de9859963a9136935f2f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/20/2020
ms.locfileid: "46820109"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.Profile.Publications["{id}"]
    .Request()
    .DeleteAsync();

```