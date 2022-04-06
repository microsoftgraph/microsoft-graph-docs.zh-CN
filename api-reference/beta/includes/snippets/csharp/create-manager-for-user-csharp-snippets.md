---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b6bfa6274eaa6329fd294384fc6203f492f505a3
ms.sourcegitcommit: 0d6d39dd6450e0c5fd6844cb78aead00a0782e46
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2022
ms.locfileid: "63758786"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Users["{user-id}"].Manager.Reference
    .Request()
    .PutAsync("6ea91a8d-e32e-41a1-b7bd-d2d185eed0e0");

```