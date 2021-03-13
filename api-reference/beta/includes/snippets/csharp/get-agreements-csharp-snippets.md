---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3b1e466f3e3fa63c36b880d07b79031cef7ae9a1
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50773954"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var agreements = await graphClient.IdentityGovernance.TermsOfUse.Agreements
    .Request()
    .GetAsync();

```