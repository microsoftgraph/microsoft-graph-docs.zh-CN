---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1f301f98dfbacc11067c52448a32a29555303b72
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50771384"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var printOperation = await graphClient.Print.Operations["{printOperation-id}"]
    .Request()
    .GetAsync();

```