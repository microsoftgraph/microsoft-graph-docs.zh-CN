---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b4f0897bcc9fddf2746973a26b25f68ec82729263039b0fc0611efa54ac1fde8
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57103894"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

CalendarCollectionPage calendars = graphClient.me().calendarGroups("{id}").calendars()
    .buildRequest()
    .get();

```