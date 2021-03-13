---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0eeacb33365513ee63df00188d5c43c7dff30d14
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50782902"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var profileCardProperties = await graphClient.Organization["{organization-id}"].Settings.ProfileCardProperties
    .Request()
    .GetAsync();

```