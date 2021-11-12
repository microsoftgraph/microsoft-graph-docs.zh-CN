---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 91b519c3e5266e8b0b644e7d1590871a4ee9310d7a531ec418e60e4000ccdd23
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57163376"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var favoritePlans = await graphClient.Me.Planner.FavoritePlans
    .Request()
    .GetAsync();

```