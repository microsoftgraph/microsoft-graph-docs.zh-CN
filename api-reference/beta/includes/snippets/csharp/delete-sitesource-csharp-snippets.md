---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b8ddf3a9cc632b36f31682fbf3573efd4afd8f33
ms.sourcegitcommit: f9f95402b8a15152ede90dd736b03d532204fc2e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/11/2020
ms.locfileid: "49659579"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Compliance.Ediscovery.Cases["4c8f8f70-7785-4bd4-b296-c98376a2c5e1"].Custodians["2192ca408ea2410eba3bec8ae873be6b"].SiteSources["38304445-3741-3333-4233-344238454333"]
    .Request()
    .DeleteAsync();

```