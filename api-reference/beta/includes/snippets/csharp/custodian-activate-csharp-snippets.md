---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2501af10ed0b932b1e59396893418dcda8102ba0
ms.sourcegitcommit: f9f95402b8a15152ede90dd736b03d532204fc2e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/11/2020
ms.locfileid: "49659354"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Compliance.Ediscovery.Cases["2192ca408ea2410eba3bec8ae873be6b"].Custodians["45454331323337443946343043464239"]
    .Activate()
    .Request()
    .PostAsync();

```