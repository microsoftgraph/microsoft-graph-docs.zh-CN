---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 516b620d25cbecfa6bc49ce8677931de4c9ea5b94bb62b68ad8a4daf178d2c2a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57103854"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var my = await graphClient.PrivilegedRoleAssignments
    .My()
    .Request()
    .GetAsync();

```