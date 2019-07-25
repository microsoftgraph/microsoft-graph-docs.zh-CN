---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7c4b94066a67c547fe9eb74290a0bbdd00c54900
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35880749"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ICalendarCollectionPage calendars = graphClient.me().calendars()
    .buildRequest()
    .get();

```