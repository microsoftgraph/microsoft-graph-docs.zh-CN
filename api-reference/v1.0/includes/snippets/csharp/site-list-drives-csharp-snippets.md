---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4cb0fd2abba83126485ff7cc5b51766052c20e2f
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50802769"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var drives = await graphClient.Sites["{site-id}"].Drives
    .Request()
    .GetAsync();

```