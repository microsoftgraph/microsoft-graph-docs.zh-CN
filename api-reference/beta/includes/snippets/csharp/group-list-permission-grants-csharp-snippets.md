---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3bada9522e05456be2a3b74b21cd79c29bf32fb8
ms.sourcegitcommit: fe1b4d098af604cc34596f595e799911ea672532
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/07/2021
ms.locfileid: "51611362"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var permissionGrants = await graphClient.Groups["{group-id}"].PermissionGrants
    .Request()
    .GetAsync();

```