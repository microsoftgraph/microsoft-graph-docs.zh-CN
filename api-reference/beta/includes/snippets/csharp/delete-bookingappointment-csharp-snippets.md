---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 12983dc99f7cb5cf592291fead02d5f853824f96
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48615139"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.BookingBusinesses["Contosolunchdelivery@M365B489948.onmicrosoft.com"].Appointments["AAMkADKqAAA="]
    .Request()
    .DeleteAsync();

```