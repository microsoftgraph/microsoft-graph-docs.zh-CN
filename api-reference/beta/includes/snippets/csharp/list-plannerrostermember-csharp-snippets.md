---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1b19d6401a5ede8151667e234d454c22c471a1085b7578a11f7a771595c37515
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57328760"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var members = await graphClient.Planner.Rosters["{plannerRoster-id}"].Members
    .Request()
    .GetAsync();

```