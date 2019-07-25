---
description: 自动生成的文件。 不修改
ms.openlocfilehash: c4f29f103d61257b85331925e8799d80c44f70a3
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35709559"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.BookingBusinesses["Contosolunchdelivery@M365B489948.onmicrosoft.com"]
    .Unpublish(bookingBusiness)
    .Request()
    .PostAsync();

```