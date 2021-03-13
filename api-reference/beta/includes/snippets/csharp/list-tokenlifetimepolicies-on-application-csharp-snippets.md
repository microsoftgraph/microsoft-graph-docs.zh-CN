---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 51afd87d342c6a08c1978d69fe50848561443359
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50786306"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var tokenLifetimePolicies = await graphClient.Applications["{application-id}"].TokenLifetimePolicies
    .Request()
    .GetAsync();

```