---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a1d02b94d89d86b69a2b98b6b1274797cce5b197b4a113a474839366939ad223
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56904020"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var healthOverviews = await graphClient.Admin.ServiceAnnouncement.HealthOverviews
    .Request()
    .Expand("issues")
    .GetAsync();

```