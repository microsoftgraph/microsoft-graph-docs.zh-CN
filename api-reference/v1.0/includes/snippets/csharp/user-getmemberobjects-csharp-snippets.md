---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 79441896785e377d1ab60a909c45e57b8f50280bb1e1df2edeab36295a64aca3
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56903212"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var securityEnabledOnly = true;

await graphClient.Me
    .GetMemberObjects(securityEnabledOnly)
    .Request()
    .PostAsync();

```