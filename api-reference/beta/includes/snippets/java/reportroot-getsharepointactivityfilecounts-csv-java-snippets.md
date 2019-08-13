---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 9077711d3ed7177e19042b0978218b7844f53196
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36359841"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ISiteActivitySummaryCollectionPage getSharePointActivityFileCounts = graphClient.reports()
    .getSharePointActivityFileCounts("D7")
    .buildRequest()
    .get();

```