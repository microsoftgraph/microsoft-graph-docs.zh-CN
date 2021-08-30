---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 01d77f02a1676cb150600f3323b6413a72a05c4fc63de188f3cba9f7b930f4b9
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56903417"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var permissionGrants = await graphClient.Groups["{group-id}"].PermissionGrants
    .Request()
    .GetAsync();

```