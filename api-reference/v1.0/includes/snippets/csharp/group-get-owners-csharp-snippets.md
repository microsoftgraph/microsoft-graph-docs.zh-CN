---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f3076e4d98ae3b88dd546cf1c2e39069fd8c81d1
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50792528"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var owners = await graphClient.Groups["{group-id}"].Owners
    .Request()
    .GetAsync();

```