---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a3e073ec523679aa8dea62366f6473aa19b59cf1
ms.sourcegitcommit: 239db9e961e42b505f52de9859963a9136935f2f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/20/2020
ms.locfileid: "46819340"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var certifications = await graphClient.Me.Profile.Certifications
    .Request()
    .GetAsync();

```