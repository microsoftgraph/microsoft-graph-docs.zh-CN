---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 24ad268575090a76b5ad7ec0d80fe7da28dd2e12c6861a06dae7253a00b75e96
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56903273"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var roleAssignmentSchedules = await graphClient.RoleManagement.Directory.RoleAssignmentSchedules
    .Request()
    .GetAsync();

```