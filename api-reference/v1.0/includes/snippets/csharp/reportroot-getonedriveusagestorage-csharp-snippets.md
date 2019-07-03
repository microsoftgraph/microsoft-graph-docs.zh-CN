---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 00b473e7c151acf9442a5e6e71dc7d87480f279b
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35492975"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var report = await graphClient.Reports.GetOneDriveUsageStorage('D7')
    .Request()
    .GetAsync();

```