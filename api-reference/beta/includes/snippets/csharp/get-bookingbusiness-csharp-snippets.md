---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 697cb5463720e7d604110d9d9ce3f357f17b8b29
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48609569"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var bookingBusiness = await graphClient.BookingBusinesses["Fabrikam@M365B489948.onmicrosoft.com"]
    .Request()
    .GetAsync();

```