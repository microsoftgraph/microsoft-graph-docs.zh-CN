---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 4fd29caed863a2f9fff82ac0c5d9038d21da1a40
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34473741"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var bookingService = await graphClient.BookingBusinesses["Contosolunchdelivery@M365B489948.onmicrosoft.com"].Services["57da6774-a087-4d69-b0e6-6fb82c339976"]
    .Request()
    .GetAsync();

```