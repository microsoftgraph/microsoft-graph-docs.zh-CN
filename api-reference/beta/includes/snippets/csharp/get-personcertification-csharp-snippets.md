---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1757948bca0e81e261a6e6027c35cab743f89eca
ms.sourcegitcommit: 239db9e961e42b505f52de9859963a9136935f2f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/20/2020
ms.locfileid: "46819669"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var personCertification = await graphClient.Me.Profile.Certifications["{id}"]
    .Request()
    .GetAsync();

```