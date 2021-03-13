---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5b31d53a746fb51c55868cc11793baf05d4156e1
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50800268"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var securityAction = await graphClient.Security.SecurityActions["{securityAction-id}"]
    .Request()
    .GetAsync();

```