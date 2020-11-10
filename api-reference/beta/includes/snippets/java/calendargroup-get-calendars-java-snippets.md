---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a4d2dbb4b4a9d80b7e16b6da98ecd84af752cf83
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48959919"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ICalendarCollectionPage calendars = graphClient.me().calendarGroups("{id}").calendars()
    .buildRequest()
    .get();

```