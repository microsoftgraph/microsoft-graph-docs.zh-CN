---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1226de3649b7ab81aa9723479551fa24db15bf3b97a8422d8c32585edfdf7c0e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57106093"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ReportRootGetUserArchivedPrintJobsCollectionPage getUserArchivedPrintJobs = graphClient.print().reports()
    .getUserArchivedPrintJobs(ReportRootGetUserArchivedPrintJobsParameterSet
        .newBuilder()
        .withUserId("016b5565-3bbf-4067-b9ff-4d68167eb1a6")
        .withStartDateTime("2021-05-24")
        .withEndDateTime("2021-05-25")
        .build())
    .buildRequest()
    .get();

```