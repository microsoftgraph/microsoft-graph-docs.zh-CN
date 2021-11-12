---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8a8d1bb09e0d5259a58b95d4f4b86bb3dcf4f7637675a83abfdc1fcb8ea76a1a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57161515"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.ServicePrincipals["{servicePrincipal-id}"].Owners["{directoryObject-id}"].Reference
    .Request()
    .DeleteAsync();

```