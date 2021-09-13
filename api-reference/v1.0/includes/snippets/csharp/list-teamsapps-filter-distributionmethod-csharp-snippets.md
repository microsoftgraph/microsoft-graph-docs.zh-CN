---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7b72d18f77bfd07087c5a84e5d0206221dbcfc057f274b16be76e6ea0206cb37
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57219391"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var teamsApps = await graphClient.AppCatalogs.TeamsApps
    .Request()
    .Filter("distributionMethod eq 'organization'")
    .GetAsync();

```