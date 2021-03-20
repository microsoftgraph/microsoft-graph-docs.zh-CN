---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5ebf18abfbf5f7f3e6a27c1960a4996227399af6
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50944018"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var stream = await graphClient.Organization["{organization-id}"].Branding.BannerLogo
    .Request()
    .Header("Accept-Language","fr")
    .GetAsync();

```