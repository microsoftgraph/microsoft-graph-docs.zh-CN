---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2c4fdec72eaff7707896590dc09fd87bab8bdcce6af81e106a33dac473ea3915
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57103831"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var transitiveMemberOf = await graphClient.ServicePrincipals["{servicePrincipal-id}"].TransitiveMemberOf
    .Request()
    .GetAsync();

```