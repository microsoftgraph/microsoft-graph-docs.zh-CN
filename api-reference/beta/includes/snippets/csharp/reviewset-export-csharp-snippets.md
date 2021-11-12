---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 432eae4ef41dd4b7cd5976150f8f8687994855eb1b0f60389b75a21928d620c3
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57105801"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var outputName = "2020-12-06 Contoso investigation export";

var description = "Export for the Contoso investigation";

var exportOptions = Microsoft.Graph.Ediscovery.ExportOptions.OriginalFiles | Microsoft.Graph.Ediscovery.ExportOptions.FileInfo | Microsoft.Graph.Ediscovery.ExportOptions.Tags;

var exportStructure = Microsoft.Graph.Ediscovery.ExportFileStructure.Directory;

await graphClient.Compliance.Ediscovery.Cases["{ediscovery.case-id}"].ReviewSets["{ediscovery.reviewSet-id}"]
    .Export(exportStructure,outputName,description,null,null,exportOptions)
    .Request()
    .PostAsync();

```