---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 05b15221670bd08c93a0b2c814e58d01d5400c68f46d35256efd05147491aa55
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57104003"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var @case = new Microsoft.Graph.Ediscovery.Case
{
    DisplayName = "My Case 1 - Renamed",
    Description = "Updated description",
    ExternalId = "Updated externalId"
};

await graphClient.Compliance.Ediscovery.Cases["{ediscovery.case-id}"]
    .Request()
    .UpdateAsync(@case);

```