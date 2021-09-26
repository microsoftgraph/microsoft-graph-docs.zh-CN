---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f1b0fa3bfebcd41cd42ac42576a244bd50dc1243
ms.sourcegitcommit: 08e9b0bac39c1b1d2c8a79539d24aaa93364baf2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/24/2021
ms.locfileid: "59763934"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var organizationSettings = await graphClient.Organization["{organization-id}"].Settings
    .Request()
    .GetAsync();

```