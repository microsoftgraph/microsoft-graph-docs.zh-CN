---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 068a13d0dcf7363f118a0504be9c630154cf063b
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50771321"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var printService = await graphClient.Print.Services["{printService-id}"]
    .Request()
    .GetAsync();

```