---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 93c53657b6f66d858b7e355d2e7850d7f21dcdc03cb9aea0de89869981b30aa8
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57218568"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var sourceCollection = new Microsoft.Graph.Ediscovery.SourceCollection
{
    Id = "1a9b4145d8f84e39bc45a7f68c5c5119"
};

var additionalData = Microsoft.Graph.Ediscovery.AdditionalDataOptions.LinkedFiles;

await graphClient.Compliance.Ediscovery.Cases["{ediscovery.case-id}"].ReviewSets["{ediscovery.reviewSet-id}"]
    .AddToReviewSet(sourceCollection,additionalData)
    .Request()
    .PostAsync();

```