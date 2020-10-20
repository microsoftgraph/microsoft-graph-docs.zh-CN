---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d1806b82098ee9d08f5bea3afe79f1d72a94256f
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48606908"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var ownedDevices = await graphClient.Me.OwnedDevices
    .Request()
    .GetAsync();

```