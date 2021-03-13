---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d7e4368250acb02cb632439ea547b80094b80d6b
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50798813"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.Profile.Positions["{workPosition-id}"]
    .Request()
    .DeleteAsync();

```