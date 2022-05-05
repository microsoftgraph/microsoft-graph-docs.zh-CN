---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ed016be81060fa5a6ab6e1c06e57e6060c432476
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65205514"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getStaffAvailability = await graphClient.BookingBusinesses["{bookingBusiness-id}"]
    .GetStaffAvailability()
    .Request()
    .GetAsync();

```