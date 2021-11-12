---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 762ba2fc8c334ed0a25f8779ec4a55d4029781dfa07864a844c952248501edec
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57220591"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var createdObjects = await graphClient.ServicePrincipals["{servicePrincipal-id}"].CreatedObjects
    .Request()
    .GetAsync();

```