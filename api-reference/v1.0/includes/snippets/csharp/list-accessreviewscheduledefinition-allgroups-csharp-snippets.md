---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a0cd5b820e2ea2b3637ab10979d9d9cd6eab3688befee72b1808e21390aaeb59
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57104632"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var definitions = await graphClient.IdentityGovernance.AccessReviews.Definitions
    .Request()
    .Filter("contains(scope/microsoft.graph.accessReviewQueryScope/query, './members')")
    .GetAsync();

```