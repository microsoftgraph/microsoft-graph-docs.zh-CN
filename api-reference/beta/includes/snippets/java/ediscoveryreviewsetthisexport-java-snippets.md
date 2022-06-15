---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e859d8be5e28b1b91f898de5627d326457bbff65
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2022
ms.locfileid: "66092385"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String outputName = "Export via API";

String description = "Export for the Contoso investigation";

EnumSet<ExportOptions> exportOptions = EnumSet.of(ExportOptions.ORIGINAL_FILES,ExportOptions.FILE_INFO,ExportOptions.TAGS);

ExportFileStructure exportStructure = ExportFileStructure.DIRECTORY;

graphClient.security().cases().ediscoveryCases("58399dff-cebe-478f-b1af-d3227f1fd645").reviewSets("273f11a1-17aa-419c-981d-ff10d33e420f")
    .export(EdiscoveryReviewSetExportParameterSet
        .newBuilder()
        .withOutputName(outputName)
        .withDescription(description)
        .withAzureBlobContainer(null)
        .withAzureBlobToken(null)
        .withExportOptions(exportOptions)
        .withExportStructure(exportStructure)
        .build())
    .buildRequest()
    .post();

```