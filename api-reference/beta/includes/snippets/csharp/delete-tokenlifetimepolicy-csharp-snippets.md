---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9dc582e087ab6280e9b54173b9c5a09de7930e4aad9f9f1e26045c58ae10787f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57332358"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Policies.TokenLifetimePolicies["{tokenLifetimePolicy-id}"]
    .Request()
    .DeleteAsync();

```