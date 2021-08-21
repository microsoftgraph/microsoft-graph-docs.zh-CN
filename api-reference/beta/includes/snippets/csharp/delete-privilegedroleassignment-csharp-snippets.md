---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 443f9c15bc21bc4357eaae659d5225360257e5cba4a662d1f20ec08a1f14cc8b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56904230"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.PrivilegedRoleAssignments["{privilegedRoleAssignment-id}"]
    .Request()
    .DeleteAsync();

```