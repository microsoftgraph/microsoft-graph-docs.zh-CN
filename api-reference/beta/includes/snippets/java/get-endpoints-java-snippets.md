---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c7eca49c98e0fe203933bd0aac5740f46312f1be
ms.sourcegitcommit: 6ec748ef00d025ee216274a608291be3c1257777
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/27/2021
ms.locfileid: "50015905"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ReportRoot reportRoot = graphClient.print().reports("dailyPrintUsageSummariesByPrinter")
    .buildRequest()
    .get();

```