---
description: 自动生成的文件。 不修改
ms.openlocfilehash: f25e4abdc267e2625481c248a9372aed2b436f2c
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35709322"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var bookingStaffMember = await graphClient.BookingBusinesses["Contosolunchdelivery@M365B489948.onmicrosoft.com"].StaffMembers["71d64d0e-7225-49b6-b0b1-070d476cda51"]
    .Request()
    .GetAsync();

```