---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e124f01b188bde80fcb765313bba455e64e81659
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50793512"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Identity.ConditionalAccess.NamedLocations["{namedLocation-id}"]
    .Request()
    .DeleteAsync();

```