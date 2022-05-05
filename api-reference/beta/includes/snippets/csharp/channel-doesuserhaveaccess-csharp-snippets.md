---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 08b31361cba2980fd84637c0d6dd4241b811f1df
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65211044"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var boolean = await graphClient.Teams["{team-id}"].Channels["{channel-id}"]
    .DoesUserHaveAccess("6285581g-484b-4845-9e01-60667f8b12ae")
    .Request()
    .GetAsync();

```