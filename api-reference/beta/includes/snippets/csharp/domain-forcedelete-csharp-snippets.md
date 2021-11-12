---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8d79feb9dd2b75f4c41838b83f66c1c6ad417c00e1eba1138e6a410f3784d5ac
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57274406"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var disableUserAccounts = true;

await graphClient.Domains["{domain-id}"]
    .ForceDelete(disableUserAccounts)
    .Request()
    .PostAsync();

```