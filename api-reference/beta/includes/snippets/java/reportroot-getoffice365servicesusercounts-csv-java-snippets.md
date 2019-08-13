---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 2e9612b2d9f01828192de2dde497df602c2ab13c
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36360263"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IOffice365ServicesUserCountsCollectionPage getOffice365ServicesUserCounts = graphClient.reports()
    .getOffice365ServicesUserCounts("D7")
    .buildRequest()
    .get();

```