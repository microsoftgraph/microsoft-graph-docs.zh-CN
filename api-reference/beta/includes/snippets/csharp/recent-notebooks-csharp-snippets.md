---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 99290b1ad913ae023a450e25b0d066247f8a8512
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50772504"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getrecentnotebooks = await graphClient.Me.Onenote.Notebooks
    .Getrecentnotebooks(true)
    .Request()
    .GetAsync();

```