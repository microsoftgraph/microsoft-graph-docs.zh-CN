---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1fb11948f966d640f7ec383da97a7bc66edfdf5d
ms.sourcegitcommit: 5a1373f2ccd9ee813fc60d42e7ac6b115b5f9f66
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/21/2020
ms.locfileid: "44338826"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Oauth2PermissionGrants["{id}"]
    .Request()
    .DeleteAsync();

```