---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 832c66862a9eb029d1a5fc1d62dee261eb5de107
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34438901"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.BookingBusinesses["Contosolunchdelivery@M365B489948.onmicrosoft.com"].Customers["80b5ddda-1e3b-4c9d-abe2-d606cc075e2e"]
    .Request()
    .DeleteAsync();

```