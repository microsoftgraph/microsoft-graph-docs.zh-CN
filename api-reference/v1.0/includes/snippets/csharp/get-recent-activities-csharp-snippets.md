---
description: 自动生成的文件。 不修改
ms.openlocfilehash: bcaab345dffb05ab00cfda6bf015ac1a94bd2ce6
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35509522"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var recent = await graphClient.Me.Activities.Recent()
    .Request()
    .GetAsync();

```