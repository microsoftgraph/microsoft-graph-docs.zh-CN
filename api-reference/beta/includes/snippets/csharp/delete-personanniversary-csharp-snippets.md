---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 72725f3194f41ddcd89221a74645748d69feb21388e6304dd9b1212713efacb2
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57161187"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.Profile.Anniversaries["{personAnnualEvent-id}"]
    .Request()
    .DeleteAsync();

```