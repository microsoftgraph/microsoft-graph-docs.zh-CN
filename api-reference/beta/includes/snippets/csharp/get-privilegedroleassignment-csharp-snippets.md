---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 499f4306ccfe9b70babc6e17df6ec30f2e923594c7635a6f15ae7e8497e7c501
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57106875"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var privilegedRoleAssignment = await graphClient.PrivilegedRoleAssignments["{privilegedRoleAssignment-id}"]
    .Request()
    .GetAsync();

```