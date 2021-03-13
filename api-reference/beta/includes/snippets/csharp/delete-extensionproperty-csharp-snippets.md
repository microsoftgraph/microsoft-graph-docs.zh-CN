---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4d6e36f8c50e43058a2435e494f9120bc20b6506
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50806053"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Applications["{application-id}"].ExtensionProperties["{extensionProperty-id}"]
    .Request()
    .DeleteAsync();

```