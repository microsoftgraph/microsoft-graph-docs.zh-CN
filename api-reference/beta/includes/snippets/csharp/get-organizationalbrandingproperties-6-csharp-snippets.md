---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5ba4a0eb4af47a056d69eef1a8477058b6e6c2d2
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50944015"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var stream = await graphClient.Organization["{organization-id}"].Branding.BannerLogo
    .Request()
    .Header("Accept-Language","de")
    .GetAsync();

```