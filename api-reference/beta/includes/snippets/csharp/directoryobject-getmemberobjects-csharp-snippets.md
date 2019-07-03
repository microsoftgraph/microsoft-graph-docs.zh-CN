---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 33f9d42a98d86a655d9644d3150c9c591244b79f
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35520075"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var securityEnabledOnly = true;

await graphClient.Me
    .GetMemberObjects(securityEnabledOnly)
    .Request()
    .PostAsync();

```