---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a3123cab04be0e18d8ac239a0c44e41c9e104ed76e26f2862a9606dbb0cfc20b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57161603"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var tokenIssuancePolicies = await graphClient.Policies.TokenIssuancePolicies
    .Request()
    .GetAsync();

```