---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8b0d62038430008c7d73aaf07827b2d5e7a2eb85
ms.sourcegitcommit: 6ec748ef00d025ee216274a608291be3c1257777
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/27/2021
ms.locfileid: "50015130"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var classes = await graphClient.Education.Classes
    .Request()
    .GetAsync();

```