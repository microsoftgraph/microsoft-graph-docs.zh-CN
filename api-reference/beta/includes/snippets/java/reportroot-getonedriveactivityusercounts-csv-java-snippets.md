---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 16a7cd32d1b9fb418fb3a913225568bd76c2cfa4
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36360047"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ISiteActivitySummaryCollectionPage getOneDriveActivityUserCounts = graphClient.reports()
    .getOneDriveActivityUserCounts("D7")
    .buildRequest()
    .get();

```