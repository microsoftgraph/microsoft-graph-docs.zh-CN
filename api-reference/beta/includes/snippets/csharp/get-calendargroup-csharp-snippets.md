---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b0367099abeb3df7ab51b8e974f5842bc26b0b2b2b039f8524c1760fe8e163e4
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57106954"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var calendarGroup = await graphClient.Me.CalendarGroups["{calendarGroup-id}"]
    .Request()
    .GetAsync();

```