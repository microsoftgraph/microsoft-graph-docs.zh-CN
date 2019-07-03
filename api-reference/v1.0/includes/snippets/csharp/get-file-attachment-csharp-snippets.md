---
description: 自动生成的文件。 不修改
ms.openlocfilehash: e350960691e1e3069ecf9fb1717daa13b99e7a2c
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35467976"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var attachment = await graphClient.Me.Events["{id}"].Attachments["{id}"]
    .Request()
    .GetAsync();

```