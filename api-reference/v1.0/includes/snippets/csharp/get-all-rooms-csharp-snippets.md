---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2f7ede6240351e046a503e8a0db7c2ccdd07d207
ms.sourcegitcommit: c650b95ef4d0c3e93e2eb36cd6b52ed31200164f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/10/2020
ms.locfileid: "44685212"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var room = await graphClient.Places
    .Request()
    .GetAsync();

```