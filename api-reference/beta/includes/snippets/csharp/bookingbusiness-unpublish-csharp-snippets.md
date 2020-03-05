---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fee9efd56dd7cb14a863a8577196a844f8320dad
ms.sourcegitcommit: 46ee19b244349e2a1537f0c44c576d7c01cf03a9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/05/2019
ms.locfileid: "37402135"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.BookingBusinesses["Contosolunchdelivery@M365B489948.onmicrosoft.com"]
    .Unpublish()
    .Request()
    .PostAsync();

```