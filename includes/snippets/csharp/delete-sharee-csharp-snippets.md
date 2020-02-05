---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 91d6a53badffede7af60a23ec63e7cb34af19a73
ms.sourcegitcommit: 7b286637aa332cfd534a41526950b4f6272e0fd7
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/05/2020
ms.locfileid: "41774803"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Users["AlexW@contoso.OnMicrosoft.com"].Calendars["AAMkADAwAABf02bAAAA="].CalendarPermissions["L289RXhjaGFuZ2VMYWJTWVnYW5C"]
    .Request()
    .DeleteAsync();

```