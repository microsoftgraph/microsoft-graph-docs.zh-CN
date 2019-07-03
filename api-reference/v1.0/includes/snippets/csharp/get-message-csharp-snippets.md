---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 5e102b8e344382e52946d5d423ce742f0228e456
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35509790"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var message = await graphClient.Me.Messages["AAMkADhMGAAA="]
    .Request()
    .GetAsync();

```