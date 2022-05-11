---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 254965554b9c8d790bad85ac9cccf10d2303c011
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65315812"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var richLongRunningOperation = await graphClient.Sites["{site-id}"].Operations["{richLongRunningOperation-id}"]
    .Request()
    .GetAsync();

```