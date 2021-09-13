---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b1ab8f5fce73d5078f89b1343526d577be1367a36cf2fce038c895bf44c74bb3
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57162031"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var stream = await graphClient.Organization["{organization-id}"].Branding.BannerLogo
    .Request()
    .Header("Accept-Language","de")
    .GetAsync();

```