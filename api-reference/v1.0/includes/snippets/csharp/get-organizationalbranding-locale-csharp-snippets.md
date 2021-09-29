---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b0a1368ca4df70eaa8800b4e37db16577b5da3e0
ms.sourcegitcommit: 36bae3615df41876493b25da478e589d1974f97b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/29/2021
ms.locfileid: "59997084"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var organizationalBranding = await graphClient.Organization["{organization-id}"].Branding
    .Request()
    .Header("Accept-Language","fr-FR")
    .GetAsync();

```