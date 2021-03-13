---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f714d2269497cd40c69e33785ff4d4a178186248
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50776513"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var sourceCollection = new Microsoft.Graph.Ediscovery.SourceCollection
{
    DisplayName = "Quarterly Financials search"
};

await graphClient.Compliance.Ediscovery.Cases["{ediscovery.case-id}"].SourceCollections["{ediscovery.sourceCollection-id}"]
    .Request()
    .UpdateAsync(sourceCollection);

```