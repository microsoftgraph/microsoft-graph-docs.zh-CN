---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bea5a238c3694818871e2d3138f2fa8319fb83bba8f70967f1e45e69ffe4b3db
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57106286"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var profileCardProperty = await graphClient.Organization["{organization-id}"].Settings.ProfileCardProperties["{profileCardProperty-id}"]
    .Request()
    .GetAsync();

```