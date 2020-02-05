---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7c4b94066a67c547fe9eb74290a0bbdd00c54900
ms.sourcegitcommit: 7b286637aa332cfd534a41526950b4f6272e0fd7
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/05/2020
ms.locfileid: "41774633"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ICalendarCollectionPage calendars = graphClient.me().calendars()
    .buildRequest()
    .get();

```