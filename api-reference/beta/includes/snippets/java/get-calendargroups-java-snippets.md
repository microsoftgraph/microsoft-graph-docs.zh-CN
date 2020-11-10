---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8316751d3ce898d35595c8141b8472f87ffcbd2d
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48979409"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ICalendarGroupCollectionPage calendarGroups = graphClient.me().calendarGroups()
    .buildRequest()
    .get();

```