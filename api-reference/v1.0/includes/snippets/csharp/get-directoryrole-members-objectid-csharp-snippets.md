---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6a8de6f5fe5a1f218ff689ca98d01fd9ab150341
ms.sourcegitcommit: 9f88b7e41a4a4a4d5f52bd995ce07c6f702bd5d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/01/2020
ms.locfileid: "49524564"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var members = await graphClient.DirectoryRoles["23f3b4b4-8a29-4420-8052-e4950273bbda"].Members
    .Request()
    .GetAsync();

```