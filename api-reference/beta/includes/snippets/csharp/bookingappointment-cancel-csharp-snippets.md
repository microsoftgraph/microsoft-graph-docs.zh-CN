---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: da19b709b8e032bed05e119d52dc97f7a6e34ee0
ms.sourcegitcommit: 46ee19b244349e2a1537f0c44c576d7c01cf03a9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/05/2019
ms.locfileid: "37402143"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var cancellationMessage = "Your appointment has been successfully cancelled. Please call us again.";

await graphClient.BookingBusinesses["Contosolunchdelivery@M365B489948.onmicrosoft.com"].Appointments["AAMkADKoAAA="]
    .Cancel(cancellationMessage)
    .Request()
    .PostAsync();

```