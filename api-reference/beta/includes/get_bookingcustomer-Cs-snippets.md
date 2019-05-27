---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 88b1c490792047e4c9a25fcec833912ab5cc984f
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34473727"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var bookingCustomer = await graphClient.BookingBusinesses["Contosolunchdelivery@M365B489948.onmicrosoft.com"].Customers["8bb19078-0f45-4efb-b2c5-da78b860f73a"]
    .Request()
    .GetAsync();

```