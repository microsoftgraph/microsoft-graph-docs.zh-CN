---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a1b5a3c4719b152bb2ffca8234ff821e27d13d1d
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50799758"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var personName = await graphClient.Me.Profile.Names["{personName-id}"]
    .Request()
    .GetAsync();

```