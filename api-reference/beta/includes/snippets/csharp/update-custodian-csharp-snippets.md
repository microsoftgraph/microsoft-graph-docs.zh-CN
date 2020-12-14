---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8f3ec8686f891611cde1609bb87d56a89c16d3eb
ms.sourcegitcommit: f9f95402b8a15152ede90dd736b03d532204fc2e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/11/2020
ms.locfileid: "49658907"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var custodian = new Custodian
{
    ApplyHoldToSources = false
};

await graphClient.Compliance.Ediscovery.Cases["2192ca408ea2410eba3bec8ae873be6b"].Custodians["45454331323337443946343043464239"]
    .Request()
    .UpdateAsync(custodian);

```