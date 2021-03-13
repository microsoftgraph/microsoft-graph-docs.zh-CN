---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e8bf4bfb711d91d60376012ec1513e9df878f2d9
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50795293"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var resources = await graphClient.PrivilegedAccess["{privilegedAccess-id}"].Resources
    .Request()
    .GetAsync();

```