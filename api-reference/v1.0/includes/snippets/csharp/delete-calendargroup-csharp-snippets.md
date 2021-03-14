---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7bd1d427bcafe64f6c6c16162f9212343dd8a480
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50780633"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.CalendarGroups["{calendarGroup-id}"]
    .Request()
    .DeleteAsync();

```