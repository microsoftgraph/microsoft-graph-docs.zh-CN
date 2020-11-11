---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 98ce52b92fa9821c04ee34e25ed0fbcac06b5c8e
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48983594"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IOutlookUserSupportedTimeZonesCollectionPage supportedTimeZones = graphClient.me().outlook()
    .supportedTimeZones(microsoft.graph.timeZoneStandard'Iana')
    .buildRequest()
    .get();

```