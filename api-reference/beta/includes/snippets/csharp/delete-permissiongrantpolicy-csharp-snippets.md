---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b29561aa508954798fb3fbb535fab68b7b07e431f82f965a4d85d775716d7c3c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57328764"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Policies.PermissionGrantPolicies["{permissionGrantPolicy-id}"]
    .Request()
    .DeleteAsync();

```