---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4d9f81cc058534de1453959ea1775bec2cda445c
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65212145"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var internalDomainFederation = await graphClient.Domains["{domain-id}"].FederationConfiguration["{internalDomainFederation-id}"]
    .Request()
    .GetAsync();

```