---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bbfe0bf197e57446e4f6f5c68db8ab94e74a5629
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/26/2021
ms.locfileid: "52668738"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var availableProviderTypes = await graphClient.Identity.IdentityProviders
    .AvailableProviderTypes()
    .Request()
    .GetAsync();

```