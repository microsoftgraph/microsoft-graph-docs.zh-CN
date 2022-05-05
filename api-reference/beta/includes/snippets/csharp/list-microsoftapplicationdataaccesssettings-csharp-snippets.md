---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5f50e7f98dbc2c867f43a915e76d712dbfdd7e70
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65205704"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var microsoftApplicationDataAccessSettings = await graphClient.Organization["{organization-id}"].Settings.MicrosoftApplicationDataAccess
    .Request()
    .GetAsync();

```