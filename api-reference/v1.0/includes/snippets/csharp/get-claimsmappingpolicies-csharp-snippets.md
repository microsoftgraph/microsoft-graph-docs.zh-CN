---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0f6514774680f9f6ae3b1a4b0a2c10c61bf1dbebcfc5fb0df98f5e1db551979b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57332652"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var claimsMappingPolicies = await graphClient.Policies.ClaimsMappingPolicies
    .Request()
    .GetAsync();

```