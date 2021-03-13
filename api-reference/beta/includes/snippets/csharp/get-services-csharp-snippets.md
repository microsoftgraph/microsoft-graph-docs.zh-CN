---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: db815b14d5f8bb7b0979aeda7d39ae9f1954506e
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50788225"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var services = await graphClient.BookingBusinesses["{bookingBusiness-id}"].Services
    .Request()
    .GetAsync();

```