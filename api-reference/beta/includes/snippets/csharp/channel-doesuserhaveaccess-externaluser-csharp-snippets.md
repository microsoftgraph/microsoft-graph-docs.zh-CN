---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a90f9211267059223c5007766b6222c58bc3c997
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65211043"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var boolean = await graphClient.Teams["{team-id}"].Channels["{channel-id}"]
    .DoesUserHaveAccess("62855810-484b-4823-9e01-60667f8b12ae","57fb72d0-d811-46f4-8947-305e6072eaa5")
    .Request()
    .GetAsync();

```