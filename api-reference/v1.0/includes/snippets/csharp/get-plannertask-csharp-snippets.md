---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a550ad916c829752c9d04d0b791c4c1cc2493a2ee737aa2b758aa89b588ed68d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57332964"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var plannerTask = await graphClient.Planner.Tasks["{plannerTask-id}"]
    .Request()
    .GetAsync();

```