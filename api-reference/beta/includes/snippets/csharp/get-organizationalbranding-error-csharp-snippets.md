---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 37d092fd8a470dcddf47cf5192acb33dc7259e14
ms.sourcegitcommit: 0eb843a6f61f384bc28c0cce1ccb74f64bdb1fa6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/23/2021
ms.locfileid: "60562775"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var organizationalBranding = await graphClient.Organization["{organization-id}"].Branding
    .Request()
    .Header("Accept-Language","0")
    .GetAsync();

```