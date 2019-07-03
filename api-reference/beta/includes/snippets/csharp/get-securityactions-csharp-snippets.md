---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 8966cc8cff64e7e98537747be28a760e40df5ea1
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35500439"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var securityActions = await graphClient.Security.SecurityActions
    .Request()
    .GetAsync();

```