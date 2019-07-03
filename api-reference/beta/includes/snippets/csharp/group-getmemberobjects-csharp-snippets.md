---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 8b7d1a86d56b923d0e951c5ca00dfc6e21e4844c
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35500404"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var securityEnabledOnly = false;

await graphClient.Groups["{id}"]
    .GetMemberObjects(securityEnabledOnly)
    .Request()
    .PostAsync();

```