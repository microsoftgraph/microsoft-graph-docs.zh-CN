---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3bc07fa6508ac796cddc917ffa306d3bdcc26502
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50800141"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.AppCatalogs.TeamsApps["{teamsApp-id}"]
    .Request()
    .DeleteAsync();

```