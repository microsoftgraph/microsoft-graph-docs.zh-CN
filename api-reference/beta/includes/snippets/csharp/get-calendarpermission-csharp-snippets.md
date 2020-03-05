---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ee501c02f44123a6263fb28f1d9c424b6cd578e8
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "37994865"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var calendarPermission = await graphClient.Users["{id}"].Calendar.CalendarPermissions["{id}"]
    .Request()
    .GetAsync();

```