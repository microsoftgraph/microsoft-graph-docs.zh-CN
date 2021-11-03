---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7d64bbc61102ef9657c0ac37176036286cf7473948b23feefd0aa561407b6212
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57105275"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var bookingStaffMember = await graphClient.BookingBusinesses["{bookingBusiness-id}"].StaffMembers["{bookingStaffMember-id}"]
    .Request()
    .GetAsync();

```