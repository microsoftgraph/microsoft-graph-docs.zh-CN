---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7f17e9db3410c43c193646525f9e9bd41c29e581
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62132129"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var riskyUser = await graphClient.IdentityProtection.RiskyUsers["{riskyUser-id}"]
    .Request()
    .GetAsync();

```