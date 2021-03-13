---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4258ccffb0f4ebb9b98f030371bdaeb74887cc42
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50779317"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.TrustFramework.Policies["{trustFrameworkPolicy-id}"]
    .Request()
    .DeleteAsync();

```