---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ce8c1c9c0c7a7b44b01b4d0014d876573106f5f4
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50800325"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var staffMembers = await graphClient.BookingBusinesses["{bookingBusiness-id}"].StaffMembers
    .Request()
    .GetAsync();

```