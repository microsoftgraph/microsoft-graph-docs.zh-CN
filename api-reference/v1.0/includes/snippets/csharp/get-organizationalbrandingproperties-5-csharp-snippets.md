---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9bb01a9ee77303fd93f5a3e35eb84e70e9477ff460932fa2375afe41d6b1518f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57215981"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var stream = await graphClient.Organization["{organization-id}"].Branding.BannerLogo
    .Request()
    .Header("Accept-Language","fr")
    .GetAsync();

```