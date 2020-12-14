---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f230f0bdfcba01548c91396a4cf2241dacbc9d7c
ms.sourcegitcommit: f9f95402b8a15152ede90dd736b03d532204fc2e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/11/2020
ms.locfileid: "49658807"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var siteSource = await graphClient.Compliance.Ediscovery.Cases["4c8f8f70-7785-4bd4-b296-c98376a2c5e1"].Custodians["2192ca408ea2410eba3bec8ae873be6b"].SiteSources["38304445-3741-3333-4233-344238454333"]
    .Request()
    .GetAsync();

```