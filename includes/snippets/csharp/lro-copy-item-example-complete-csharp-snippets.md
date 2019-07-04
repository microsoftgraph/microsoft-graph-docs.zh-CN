---
description: 自动生成的文件。 不修改
ms.openlocfilehash: dc93bcaf0755ac9776f4e88ea0c754c09245f975
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35533266"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var driveItem = await graphClient.Me.Drive.Items["{item-id}"]
    .Request()
    .GetAsync();

```