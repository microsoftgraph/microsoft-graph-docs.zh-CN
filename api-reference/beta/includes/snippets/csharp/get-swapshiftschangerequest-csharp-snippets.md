---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 690cbfd6fe905a478290bd84e37cbc109ea6f966
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "40865049"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var swapShiftsChangeRequests = await graphClient.Teams["{id}"].Schedule.SwapShiftsChangeRequests
    .Request()
    .GetAsync();

```