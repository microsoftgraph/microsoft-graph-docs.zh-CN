---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: cebf20ac8e803a094ca1cce6208274f260b73dc0216841a5e2717e274351ea2c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57163930"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ReportRootGetGroupArchivedPrintJobsCollectionPage getGroupArchivedPrintJobs = graphClient.print().reports()
    .getGroupArchivedPrintJobs(ReportRootGetGroupArchivedPrintJobsParameterSet
        .newBuilder()
        .withGroupId("016b5565-3bbf-4067-b9ff-4d68167eb1a6")
        .withStartDateTime("2021-05-24")
        .withEndDateTime("2021-05-25")
        .build())
    .buildRequest()
    .get();

```