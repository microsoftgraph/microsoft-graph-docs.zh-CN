---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ab53de7f831828f0813f860b492f1f608876ac32ccdc1a56dacd3ff5e7aba126
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57278137"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var policies = await graphClient.Identity.ConditionalAccess.Policies
    .Request()
    .Filter("displayName eq 'SimplePolicy1' or displayName eq 'SimplePolicy2'")
    .GetAsync();

```