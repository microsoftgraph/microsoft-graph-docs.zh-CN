---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 950ff57da15267ac800bee48b9d25dfb3c3b9105fff4b1ceb46f77ba444c46f1
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57333176"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var secureScores = await graphClient.Security.SecureScores
    .Request()
    .Top(1)
    .GetAsync();

```