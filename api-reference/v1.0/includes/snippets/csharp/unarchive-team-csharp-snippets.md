---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 30fc9e88784b21e3d7a149e5321e71e9a81704b4
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50782340"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Teams["{team-id}"]
    .Unarchive()
    .Request()
    .PostAsync();

```