---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 983a9f6179590eba3a833fadd6cbdcc3a47b00c9
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48605995"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var driveItem = await graphClient.Shares["{shareIdOrUrl}"].DriveItem
    .Request()
    .Expand("children")
    .GetAsync();

```