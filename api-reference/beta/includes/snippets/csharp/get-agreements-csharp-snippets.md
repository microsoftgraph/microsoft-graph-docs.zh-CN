---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6e8b694b843e3ea93f5a93248388bd56ee79fe31f7d2db3e688fabe11a8705eb
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56902541"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var agreements = await graphClient.IdentityGovernance.TermsOfUse.Agreements
    .Request()
    .GetAsync();

```