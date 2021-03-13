---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 82c2f26cd0553f22228e428af9303dc2d1fa625c
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50794119"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var servicePrincipal = await graphClient.ServicePrincipals["{servicePrincipal-id}"]
    .Request()
    .GetAsync();

```