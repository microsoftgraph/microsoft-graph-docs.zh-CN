---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b62863a8d4bf35f53f1235063de8577355201b67bdb23e5e0f3a6f37a2f0f858
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57278393"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var custodian = new Microsoft.Graph.Ediscovery.Custodian
{
    ApplyHoldToSources = false
};

await graphClient.Compliance.Ediscovery.Cases["{ediscovery.case-id}"].Custodians["{ediscovery.custodian-id}"]
    .Request()
    .UpdateAsync(custodian);

```