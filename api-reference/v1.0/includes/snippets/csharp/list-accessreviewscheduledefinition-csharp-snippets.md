---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d1ff15e9d798f47ecf74114163db95d2a6c798a06575a99042d86b90ecfeb4c2
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56903002"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var definitions = await graphClient.IdentityGovernance.AccessReviews.Definitions
    .Request()
    .Skip(0)
    .Top(100)
    .GetAsync();

```