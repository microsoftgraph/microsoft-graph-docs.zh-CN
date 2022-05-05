---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3dea0594e29bfe369836b07b9ee5cf746cd01f19
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65211045"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var boolean = await graphClient.Teams["{team-id}"].Channels["{channel-id}"]
    .DoesUserHaveAccess("john.doe@contoso.com")
    .Request()
    .GetAsync();

```