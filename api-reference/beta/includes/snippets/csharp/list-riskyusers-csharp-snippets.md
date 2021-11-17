---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8a37e226605c34d3150b95ad44d344f0945ef5e77290e02d11b619defe167601
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56903069"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var riskyUsers = await graphClient.RiskyUsers
    .Request()
    .GetAsync();

```