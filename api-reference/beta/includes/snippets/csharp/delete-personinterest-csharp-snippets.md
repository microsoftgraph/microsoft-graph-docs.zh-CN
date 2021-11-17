---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3336cfa4e388ab8b116497c922eb41ac6526e51a4839bdd8ed2262e026fd77e3
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57163656"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.Profile.Interests["{personInterest-id}"]
    .Request()
    .DeleteAsync();

```