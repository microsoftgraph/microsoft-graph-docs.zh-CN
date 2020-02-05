---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c8ce6fd9df6ba0a7d47294dc9e9d699c81576de6
ms.sourcegitcommit: 7b286637aa332cfd534a41526950b4f6272e0fd7
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/05/2020
ms.locfileid: "41774645"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var calendars = await graphClient.Me.Calendars
    .Request()
    .GetAsync();

```