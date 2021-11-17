---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4458b1f5ed69f2041c0122c632f077448443adb5de63e1726d0c1a39863491d2
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57158463"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var templates = await graphClient.ServicePrincipals["{servicePrincipal-id}"].Synchronization.Templates
    .Request()
    .GetAsync();

```