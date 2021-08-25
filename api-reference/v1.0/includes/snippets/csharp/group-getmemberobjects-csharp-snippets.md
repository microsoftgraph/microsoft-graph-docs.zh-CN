---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 41165742d151c55f4162b5728659fccf7811a2b812d184306060fb493378c275
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57332581"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var securityEnabledOnly = false;

await graphClient.Groups["{group-id}"]
    .GetMemberObjects(securityEnabledOnly)
    .Request()
    .PostAsync();

```