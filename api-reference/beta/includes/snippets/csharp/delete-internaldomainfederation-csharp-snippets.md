---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 73c3fb1cf5059a7fe78190de71b8b2e9928e27c5
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65211780"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Domains["{domain-id}"].FederationConfiguration["{internalDomainFederation-id}"]
    .Request()
    .DeleteAsync();

```