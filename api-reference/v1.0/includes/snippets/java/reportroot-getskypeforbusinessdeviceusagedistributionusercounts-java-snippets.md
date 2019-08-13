---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 99ef6dfbd1c8940ecf892ed27b57fe8b5283cac5
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36349173"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Report report = graphClient.reports()
    .getSkypeForBusinessDeviceUsageDistributionUserCounts("D7")
    .buildRequest()
    .get();

```