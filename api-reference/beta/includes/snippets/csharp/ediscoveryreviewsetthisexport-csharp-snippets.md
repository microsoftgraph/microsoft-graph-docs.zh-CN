---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 956a362ff3497d6c98f417688a08f8225ef9e3dd
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2022
ms.locfileid: "66092384"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var outputName = "Export via API";

var description = "Export for the Contoso investigation";

var exportOptions = Microsoft.Graph.Security.ExportOptions.OriginalFiles | Microsoft.Graph.Security.ExportOptions.FileInfo | Microsoft.Graph.Security.ExportOptions.Tags;

var exportStructure = Microsoft.Graph.Security.ExportFileStructure.Directory;

await graphClient.Security.Cases.EdiscoveryCases["{security.ediscoveryCase-id}"].ReviewSets["{security.ediscoveryReviewSet-id}"]
    .Export(outputName,description,null,null,exportOptions,exportStructure)
    .Request()
    .PostAsync();

```