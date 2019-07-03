---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 9733a179d2bdc2c2d3dcd0ecec4fa86db5486b68
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35500334"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me
    .RevokeSignInSessions()
    .Request()
    .PostAsync();

```