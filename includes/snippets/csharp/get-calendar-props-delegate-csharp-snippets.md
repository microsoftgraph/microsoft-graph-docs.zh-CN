---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a6cb271e6a44a8942b313a85e4bf60e7664ed2cb
ms.sourcegitcommit: 7b286637aa332cfd534a41526950b4f6272e0fd7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/05/2020
ms.locfileid: "41774794"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var calendar = await graphClient.Users["meganb@contoso.OnMicrosoft.com"].Calendars["AAMkADlAABhbftjAAA="]
    .Request()
    .GetAsync();

```