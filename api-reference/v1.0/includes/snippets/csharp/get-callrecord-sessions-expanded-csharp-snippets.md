---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9417b4b77632ea2271ab723982e8f5df0106dbd2
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2021
ms.locfileid: "50473883"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var sessions = await graphClient.Communications.CallRecords["{id}"].Sessions
    .Request()
    .Expand("segments")
    .GetAsync();

```