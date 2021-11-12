---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4ab6dcf19aa11d10457f1fad181deb9782cc70819c5c6a680eef27a94b3bf4e8
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56904222"
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