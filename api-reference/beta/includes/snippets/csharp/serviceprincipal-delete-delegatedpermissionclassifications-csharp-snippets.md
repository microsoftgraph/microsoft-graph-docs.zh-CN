---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 85cebc3979ec52bf1f302a846e29b3ffb356ee98
ms.sourcegitcommit: be796d6a7ae62f052c381d20207545f057b184d9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/14/2020
ms.locfileid: "48458602"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.ServicePrincipals["{id}"].DelegatedPermissionClassifications["{id}"]
    .Request()
    .DeleteAsync();

```