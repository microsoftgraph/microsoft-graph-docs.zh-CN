---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3f3822e9d66b667e5ab1a419e5c373a8bd1e5ead
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50803067"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var securityEnabledOnly = false;

await graphClient.Groups["{group-id}"]
    .GetMemberObjects(securityEnabledOnly)
    .Request()
    .PostAsync();

```