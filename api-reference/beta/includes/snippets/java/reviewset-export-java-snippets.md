---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ee9cafb23e7943d03fb355c5dbdb65474743603b4c1ca40472578b116cf232ad
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57105799"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String outputName = "2020-12-06 Contoso investigation export";

String description = "Export for the Contoso investigation";

EnumSet<ExportOptions> exportOptions = EnumSet.of(ExportOptions.ORIGINAL_FILES,ExportOptions.FILE_INFO,ExportOptions.TAGS);

ExportFileStructure exportStructure = ExportFileStructure.DIRECTORY;

graphClient.compliance().ediscovery().cases("99e865fc-e29f-479a-ba83-9e58eb017103").reviewSets("e44ac2cb-f8b4-4fd8-aa1c-1391b46ba9cc")
    .export(ReviewSetExportParameterSet
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