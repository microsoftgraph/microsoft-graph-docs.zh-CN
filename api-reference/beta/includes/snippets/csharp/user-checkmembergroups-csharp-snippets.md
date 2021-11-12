---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 33d5313804b4abe2770c38238fa8fb2d6cd972b094c009c389ca84037850d73b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57106244"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var groupIds = new List<String>()
{
    "groupIds-value"
};

await graphClient.Me
    .CheckMemberGroups(groupIds)
    .Request()
    .PostAsync();

```