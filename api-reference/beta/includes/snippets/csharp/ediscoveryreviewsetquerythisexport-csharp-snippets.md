---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 63d4a1dbeae35b7b11f687e1ca09f3b62bc4875e
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2022
ms.locfileid: "66095877"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var outputName = "Export reviewset query via API";

var description = "Export for the Contoso investigation 2";

var exportOptions = Microsoft.Graph.Security.ExportOptions.OriginalFiles | Microsoft.Graph.Security.ExportOptions.FileInfo | Microsoft.Graph.Security.ExportOptions.Tags;

var exportStructure = Microsoft.Graph.Security.ExportFileStructure.Directory;

await graphClient.Security.Cases.EdiscoveryCases["{security.ediscoveryCase-id}"].ReviewSets["{security.ediscoveryReviewSet-id}"].Queries["{security.ediscoveryReviewSetQuery-id}"]
    .Export(outputName,description,null,null,exportOptions,exportStructure)
    .Request()
    .PostAsync();

```