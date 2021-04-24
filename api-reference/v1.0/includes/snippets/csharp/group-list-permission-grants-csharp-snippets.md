---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3bada9522e05456be2a3b74b21cd79c29bf32fb8
ms.sourcegitcommit: 2006bf01c60793ac6ab1e25fa0526ec5d33c6334
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/23/2021
ms.locfileid: "51961391"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var permissionGrants = await graphClient.Groups["{group-id}"].PermissionGrants
    .Request()
    .GetAsync();

```