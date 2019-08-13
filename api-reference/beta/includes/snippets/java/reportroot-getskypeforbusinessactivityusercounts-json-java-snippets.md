---
description: 自动生成的文件。 不修改
ms.openlocfilehash: d89c168b8ba48555d25000bddefc98db4d7f84be
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36359662"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ISkypeForBusinessActivityUserCountsCollectionPage getSkypeForBusinessActivityUserCounts = graphClient.reports()
    .getSkypeForBusinessActivityUserCounts("D7")
    .buildRequest()
    .get();

```