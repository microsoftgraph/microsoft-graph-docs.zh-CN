---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 57a685f4b68deb93b31a148541847a15b7a5212c
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50805818"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.BookingBusinesses["{bookingBusiness-id}"]
    .Publish()
    .Request()
    .PostAsync();

```