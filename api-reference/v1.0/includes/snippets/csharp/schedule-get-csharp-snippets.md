---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 48f110f163f8b1f7b554f49cf2467a74ebe3fdfa
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50788786"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var schedule = await graphClient.Teams["{team-id}"].Schedule
    .Request()
    .GetAsync();

```