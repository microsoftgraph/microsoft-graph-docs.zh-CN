---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d572a102c591937bcd3d4b633143033b5600a03e
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50778810"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var tokenIssuancePolicies = await graphClient.Applications["{application-id}"].TokenIssuancePolicies
    .Request()
    .GetAsync();

```