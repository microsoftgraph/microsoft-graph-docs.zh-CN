---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 28a7289df6e09e87f237cd91e5f2fdba414f8d0f646f2dc4e0db07222319014e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57277522"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var rubrics = await graphClient.Education.Me.Rubrics
    .Request()
    .GetAsync();

```