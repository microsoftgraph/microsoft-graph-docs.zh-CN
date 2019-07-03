---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 360ebe3b06dcd09e484bff21fe3637cf7772d6ad
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35500266"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var activities = await graphClient.Me.Drive.Activities
    .Request()
    .GetAsync();

```