---
description: 自动生成的文件。 不修改
ms.openlocfilehash: fee9dfd6ff6c058aedeba208abc18e440acbe8ef
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36360220"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ISiteActivitySummaryCollectionPage getOneDriveActivityFileCounts = graphClient.reports()
    .getOneDriveActivityFileCounts("D7")
    .buildRequest()
    .get();

```