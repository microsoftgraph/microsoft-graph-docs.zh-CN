---
description: 自动生成的文件。 不修改
ms.openlocfilehash: bde44e2603ebab6be74016b16ad649918eaa7202
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35872939"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IOneDriveUsageFileCountsCollectionPage getOneDriveUsageFileCounts = graphClient.reports()
    .getOneDriveUsageFileCounts('D7')
    .buildRequest()
    .get();

```