---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 068488d8c730a8e5c8148f8f9ecfee2f7061bb93
ms.sourcegitcommit: 9f88b7e41a4a4a4d5f52bd995ce07c6f702bd5d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/01/2020
ms.locfileid: "49524011"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var delegatedPermissionClassifications = await graphClient.ServicePrincipals["{id}"].DelegatedPermissionClassifications
    .Request()
    .GetAsync();

```