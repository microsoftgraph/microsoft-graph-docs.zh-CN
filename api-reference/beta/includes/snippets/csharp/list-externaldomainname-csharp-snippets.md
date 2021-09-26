---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d0ce4ddf012b73c30eb1c80997b8a8897e7a7b90
ms.sourcegitcommit: 08e9b0bac39c1b1d2c8a79539d24aaa93364baf2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/24/2021
ms.locfileid: "59766516"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var domains = await graphClient.Directory.FederationConfigurations["{samlOrWsFedExternalDomainFederation-id}"].Domains
    .Request()
    .GetAsync();

```