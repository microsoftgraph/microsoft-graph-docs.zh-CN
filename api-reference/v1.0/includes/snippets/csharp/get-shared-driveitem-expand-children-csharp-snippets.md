---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 983a9f6179590eba3a833fadd6cbdcc3a47b00c9
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35467744"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var driveItem = await graphClient.Shares["{shareIdOrUrl}"].DriveItem
    .Request()
    .Expand("children")
    .GetAsync();

```