---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 02c3f82071993cb291f23adc5de4859e5114f7d4
ms.sourcegitcommit: 66c8fcafee151278f8089cd26d0c5766d33d04a8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/09/2020
ms.locfileid: "40995367"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Teams["{id}"].Schedule.OpenShifts["{openShiftId}"]
    .Request()
    .DeleteAsync();

```