---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1686d10f690ad12e33581a6eb59815f95231f65e
ms.sourcegitcommit: 503c72036c376a30e08c29df8e7730a7afcab66e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/10/2021
ms.locfileid: "52870701"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ReportRootGetPrinterArchivedPrintJobsCollectionPage getPrinterArchivedPrintJobs = graphClient.print().reports()
    .getPrinterArchivedPrintJobs(ReportRootGetPrinterArchivedPrintJobsParameterSet
        .newBuilder()
        .withPrinterId("016b5565-3bbf-4067-b9ff-4d68167eb1a6")
        .withStartDateTime("2021-05-24")
        .withEndDateTime("2021-05-25")
        .build())
    .buildRequest()
    .get();

```