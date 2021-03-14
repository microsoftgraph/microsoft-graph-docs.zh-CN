---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: da4324d22365fd197da2b5c0da5e7a93b7225e7d
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50779973"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var group = await graphClient.Groups["{group-id}"]
    .Request()
    .GetAsync();

```