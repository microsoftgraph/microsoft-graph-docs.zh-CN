---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ba574b88758b523350244434d5a2e94e978d79638866e57439160a74f8883c36
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57219207"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var b2cUserFlows = await graphClient.Identity.B2cUserFlows
    .Request()
    .GetAsync();

```