---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1ce79c261a57a731b799a4fa2bb54e978f4e1bab
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50806679"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.ServicePrincipals["{servicePrincipal-id}"]
    .Request()
    .DeleteAsync();

```