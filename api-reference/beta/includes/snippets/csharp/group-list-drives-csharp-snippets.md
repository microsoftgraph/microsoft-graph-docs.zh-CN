---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e8c4a921c00875d1ca45d6ceb2661b731c82fc08
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50793717"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var drives = await graphClient.Groups["{group-id}"].Drives
    .Request()
    .GetAsync();

```