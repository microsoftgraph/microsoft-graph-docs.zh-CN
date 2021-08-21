---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f1c62d9e37b3d2290467b4b835f3742ea9fcf8d98156d393616585a448356554
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57220755"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var securityEnabledOnly = true;

await graphClient.Me
    .GetMemberGroups(securityEnabledOnly)
    .Request()
    .PostAsync();

```