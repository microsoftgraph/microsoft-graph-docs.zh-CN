---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 12bb5dc83fd03c6b4800e4e05fa7966d10433d09
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65212539"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var allChannels = await graphClient.Teams["{team-id}"].AllChannels
    .Request()
    .Filter("membershipType eq 'shared'")
    .GetAsync();

```