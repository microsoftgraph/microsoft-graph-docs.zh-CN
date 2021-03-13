---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1373c5a8b0aec2d8e93d51f92824b0cfc2cfd5c8
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50789327"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.BookingBusinesses["{bookingBusiness-id}"]
    .Unpublish()
    .Request()
    .PostAsync();

```