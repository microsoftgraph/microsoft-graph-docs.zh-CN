---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 18ba187c8620a57cbe4d9c868d421eda73f915a2
ms.sourcegitcommit: d4114bac58628527611e83e436132c6581a19c52
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/13/2020
ms.locfileid: "35706380"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var disableUserAccounts = true;

await graphClient.Domains["contoso.com"]
    .ForceDelete(disableUserAccounts)
    .Request()
    .PostAsync();

```