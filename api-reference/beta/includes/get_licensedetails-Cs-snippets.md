---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 25c3f9dd496c2a2bb6eee627a0d0b5b8b9788ca0
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34449253"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var licenseDetails = await graphClient.Me.LicenseDetails
    .Request()
    .GetAsync();

```