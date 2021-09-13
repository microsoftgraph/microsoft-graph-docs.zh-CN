---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 93aae139444e5dfa824999a1e569834dc47d7a93efb36ef82529a6df09e1d198
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56902213"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var followedSites = await graphClient.Me.FollowedSites
    .Request()
    .GetAsync();

```