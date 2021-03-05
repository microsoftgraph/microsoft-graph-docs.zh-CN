---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c11f41d1633bee980a2f457410666b48ba26a64d
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2021
ms.locfileid: "50473913"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var sessions = await graphClient.Communications.CallRecords["{id}"].Sessions
    .Request()
    .GetAsync();

```