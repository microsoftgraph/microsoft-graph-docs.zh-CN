---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0d88665dcdf5dcabba53e3dbe08079b719e53116
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65315378"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var samlOrWsFedExternalDomainFederation = await graphClient.Directory.FederationConfigurations
    .Request()
    .Filter("domains/any(x: x/id eq 'contoso.com')")
    .GetAsync();

```