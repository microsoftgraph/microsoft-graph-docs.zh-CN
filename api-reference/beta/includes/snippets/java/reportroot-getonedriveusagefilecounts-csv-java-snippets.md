---
description: 自动生成的文件。 不修改
ms.openlocfilehash: bf8c3292f478158fa0cb76bfc2442532c527eff3
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36360026"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IOneDriveUsageFileCountsCollectionPage getOneDriveUsageFileCounts = graphClient.reports()
    .getOneDriveUsageFileCounts("D7")
    .buildRequest()
    .get();

```