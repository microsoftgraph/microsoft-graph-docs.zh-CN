---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 32255fb263677d89f84c340c7d0744cb473e0314889399434337cf5a0047c4d2
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57331927"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var sessions = await graphClient.Communications.CallRecords["{callRecords.callRecord-id}"].Sessions
    .Request()
    .Expand("segments")
    .GetAsync();

```