---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4820e78fcae36abf13ba67cd32980a86c63bfc3239603ae01082d19d7d0012e6
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56904023"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var roleDefinitions = await graphClient.RoleManagement.Directory.RoleDefinitions
    .Request()
    .GetAsync();

```