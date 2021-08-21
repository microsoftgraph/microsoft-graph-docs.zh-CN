---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7bb4ff8eeb2e2147dd39dedd0f25f767b60ed11dd30fc028dcd19c265c0ad37c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57273946"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.PrivilegedRoleAssignments["{privilegedRoleAssignment-id}"]
    .MakeEligible()
    .Request()
    .PostAsync();

```