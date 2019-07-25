---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 8316751d3ce898d35595c8141b8472f87ffcbd2d
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35889385"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ICalendarGroupCollectionPage calendarGroups = graphClient.me().calendarGroups()
    .buildRequest()
    .get();

```