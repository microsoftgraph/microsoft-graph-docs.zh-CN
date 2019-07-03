---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 857aef821e1b51555011cf3409468a75d27adaed
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35463741"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var delta = await graphClient.Me.Drive.Root.Delta('1230919asd190410jlka')
    .Request()
    .GetAsync();

```