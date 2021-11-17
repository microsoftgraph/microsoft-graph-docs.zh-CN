---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8a4f0f27f12713245e7d8c10cb4d42a2d7eac03b6868c002056c61b77bfe94f8
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57158295"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var b2xUserFlows = await graphClient.Identity.B2xUserFlows
    .Request()
    .GetAsync();

```