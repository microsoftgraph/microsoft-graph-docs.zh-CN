---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8ec3f3bb705dddfecf95ab6a0f59d3280d248641e327bf8f8c66b66a5b5df7eb
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57278654"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.Profile.Account["{userAccountInformation-id}"]
    .Request()
    .DeleteAsync();

```