---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4d88b9a757bade01331f090bbe0410a808fc6976070b57373a75c9c7ca6eb9e8
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57104566"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var securityEnabledOnly = false;

await graphClient.Contacts["{orgContact-id}"]
    .GetMemberGroups(securityEnabledOnly)
    .Request()
    .PostAsync();

```