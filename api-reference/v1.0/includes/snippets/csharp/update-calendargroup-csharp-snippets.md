---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 76b0b1ae284678085767c3d640a13f24c998abad4377ea5029b9b4c1c26224e4
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57277565"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var calendarGroup = new CalendarGroup
{
    Name = "name-value"
};

await graphClient.Me.CalendarGroups["{calendarGroup-id}"]
    .Request()
    .UpdateAsync(calendarGroup);

```