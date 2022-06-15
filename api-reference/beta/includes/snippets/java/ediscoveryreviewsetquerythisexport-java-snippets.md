---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e41e04b3fd94be4457275e0dd5794159de52e1c6
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2022
ms.locfileid: "66095878"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String outputName = "Export reviewset query via API";

String description = "Export for the Contoso investigation 2";

EnumSet<ExportOptions> exportOptions = EnumSet.of(ExportOptions.ORIGINAL_FILES,ExportOptions.FILE_INFO,ExportOptions.TAGS);

ExportFileStructure exportStructure = ExportFileStructure.DIRECTORY;

graphClient.security().cases().ediscoveryCases("58399dff-cebe-478f-b1af-d3227f1fd645").reviewSets("273f11a1-17aa-419c-981d-ff10d33e420f").queries("fcb86cd1-50e0-427c-840e-ba6f087364e5")
    .export(EdiscoveryReviewSetQueryExportParameterSet
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