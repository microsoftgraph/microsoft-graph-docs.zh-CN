---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5c237d1329c255125cc324781b7ec5dfc7a0988951e8f77741fa47476047ccff
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57105050"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var staffMembers = await graphClient.BookingBusinesses["{bookingBusiness-id}"].StaffMembers
    .Request()
    .GetAsync();

```