---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 000b4e22363e07589f35d2a4cbf34deb1bd080b1
ms.sourcegitcommit: f50b1feff72182d1e19bfa346304beaf29558b68
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/19/2019
ms.locfileid: "36461313"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var rubrics = await graphClient.Education.Me.Rubrics
    .Request()
    .GetAsync();

```