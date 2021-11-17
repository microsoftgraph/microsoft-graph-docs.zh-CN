---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a04d5a9db93c1dd24d770586449eb8a8a5887aa4bd1a9380886ef45293d1c739
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57105825"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.BookingBusinesses["{bookingBusiness-id}"].StaffMembers["{bookingStaffMember-id}"]
    .Request()
    .DeleteAsync();

```