---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 10a36f4288d6cbb00f6785379b57464104f852e8
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50789606"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Applications["{application-id}"].Owners["{directoryObject-id}"].Reference
    .Request()
    .DeleteAsync();

```