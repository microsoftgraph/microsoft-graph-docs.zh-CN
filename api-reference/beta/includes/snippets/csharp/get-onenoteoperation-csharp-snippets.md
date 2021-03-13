---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1000f423660b917cd4f3bd50ce1b197bcfcada7d
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50781189"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var onenoteOperation = await graphClient.Me.Onenote.Operations["{onenoteOperation-id}"]
    .Request()
    .GetAsync();

```