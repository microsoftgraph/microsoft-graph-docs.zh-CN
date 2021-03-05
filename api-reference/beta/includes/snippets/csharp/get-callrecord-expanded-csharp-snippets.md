---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c0c0ef59e5460c0585cfdab0a76e597898ac6e31
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2021
ms.locfileid: "50472603"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var callRecord = await graphClient.Communications.CallRecords["{id}"]
    .Request()
    .Expand("sessions($expand=segments)")
    .GetAsync();

```