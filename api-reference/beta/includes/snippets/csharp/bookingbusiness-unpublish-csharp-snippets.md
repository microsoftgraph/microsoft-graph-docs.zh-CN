---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e1f516c0d6542006531a9cda7ff08c8f4c9d03df3fd7131623c3519505a2a23d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57162104"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.BookingBusinesses["{bookingBusiness-id}"]
    .Unpublish()
    .Request()
    .PostAsync();

```