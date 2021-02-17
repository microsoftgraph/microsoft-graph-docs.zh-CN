---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4a2206ca1df6add49f2d30cacf053e46f28ffcd0
ms.sourcegitcommit: 42fdb068616222eb6b0813e93b33e830fc7eedc0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/17/2021
ms.locfileid: "50274742"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var @string = await graphClient.Education.Classes["11012"].Assignments["19002"]
    .GetResourcesFolderUrl()
    .Request()
    .GetAsync();

```