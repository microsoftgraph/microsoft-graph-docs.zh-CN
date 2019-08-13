---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 8193e9fbfe7144a5474cd04afe2f9bdb10418178
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36359618"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ISkypeForBusinessActivityCountsCollectionPage getSkypeForBusinessActivityCounts = graphClient.reports()
    .getSkypeForBusinessActivityCounts("D7")
    .buildRequest()
    .get();

```