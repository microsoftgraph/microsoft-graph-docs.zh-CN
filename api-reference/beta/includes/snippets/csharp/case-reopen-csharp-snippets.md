---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ded19085deaba2395b8addc657e421a936f3d015e7eff7f86ca74a6597276404
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57278792"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Compliance.Ediscovery.Cases["{ediscovery.case-id}"]
    .Reopen()
    .Request()
    .PostAsync();

```