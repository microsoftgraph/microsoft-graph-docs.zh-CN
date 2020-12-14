---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 46648ae400e0bde786a4f11c6b5eb2ee865517e7
ms.sourcegitcommit: f9f95402b8a15152ede90dd736b03d532204fc2e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/11/2020
ms.locfileid: "49659114"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var unifiedGroupSource = await graphClient.Compliance.Ediscovery.Cases["4c8f8f70-7785-4bd4-b296-c98376a2c5e1"].Custodians["2192ca408ea2410eba3bec8ae873be6b"].UnifiedGroupSources["33434233-3030-3739-3043-393039324633"]
    .Request()
    .GetAsync();

```