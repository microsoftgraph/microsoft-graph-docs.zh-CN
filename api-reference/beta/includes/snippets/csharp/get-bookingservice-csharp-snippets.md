---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b515f3bf588622715316732c0fd84808a0745a63
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50783128"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var bookingService = await graphClient.BookingBusinesses["{bookingBusiness-id}"].Services["{bookingService-id}"]
    .Request()
    .GetAsync();

```