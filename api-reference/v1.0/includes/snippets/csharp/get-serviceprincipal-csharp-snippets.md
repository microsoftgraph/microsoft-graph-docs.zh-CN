---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: af0fa235a7989ef0ce5ee087d9dad43ca8e3c563f87fdff1293780b9640c18b5
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57162538"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var servicePrincipal = await graphClient.ServicePrincipals["{servicePrincipal-id}"]
    .Request()
    .GetAsync();

```