---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 515da46b5d2b6f28e9d5a78594c9df939fbaebe5
ms.sourcegitcommit: 08d47a31c48fd69ae4fcee26e34fdd65ad1ba69f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/02/2021
ms.locfileid: "51573178"
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