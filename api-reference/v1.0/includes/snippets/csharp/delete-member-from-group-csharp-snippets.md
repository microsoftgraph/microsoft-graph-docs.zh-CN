---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1f159648c1fba5351a7bedfd40ac8f8c6c26f962
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50800050"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Groups["{group-id}"].Members["{directoryObject-id}"].Reference
    .Request()
    .DeleteAsync();

```