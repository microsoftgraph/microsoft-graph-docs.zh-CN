---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ec9f3965d13e6c24503c67cdc8853fb19b6fac76
ms.sourcegitcommit: 36bae3615df41876493b25da478e589d1974f97b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/29/2021
ms.locfileid: "59997032"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Organization["{organization-id}"].Branding
    .Request()
    .DeleteAsync();

```