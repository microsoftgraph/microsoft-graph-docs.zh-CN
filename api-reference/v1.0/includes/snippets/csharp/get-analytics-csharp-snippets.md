---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 023577eee33e9fa8e8702a49c156723efec01aab
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/18/2020
ms.locfileid: "44793910"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var followedSites = await graphClient.Me.FollowedSites
    .Request()
    .GetAsync();

```