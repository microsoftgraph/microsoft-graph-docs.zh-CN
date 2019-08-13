---
description: 自动生成的文件。 不修改
ms.openlocfilehash: dc4d05a5a5588ce0a6e91a404ad56b7d1b98ea16
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36359214"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ISkypeForBusinessOrganizerActivityUserCountsCollectionPage getSkypeForBusinessOrganizerActivityUserCounts = graphClient.reports()
    .getSkypeForBusinessOrganizerActivityUserCounts("D7")
    .buildRequest()
    .get();

```