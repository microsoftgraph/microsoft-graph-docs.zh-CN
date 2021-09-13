---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ff86e5f436ff10d4680f64b905502a26447d98016ffc8bfd42dc9e4d484b5d0f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57105430"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var tokenIssuancePolicies = await graphClient.Applications["{application-id}"].TokenIssuancePolicies
    .Request()
    .GetAsync();

```