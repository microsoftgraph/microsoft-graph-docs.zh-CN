---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 8e5eee0f52fdc3a57b28e08240be8321b826eab3
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35709342"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.BookingBusinesses["Contosolunchdelivery@M365B489948.onmicrosoft.com"].StaffMembers["5fae928f-6d2d-417a-ad96-4b0caeb362d6"]
    .Request()
    .DeleteAsync();

```