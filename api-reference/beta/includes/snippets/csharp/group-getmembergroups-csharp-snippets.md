---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: da72517f39a4adfa27de6d47658647d016d149f0640f926edaf0b3501bac74f6
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57219044"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var securityEnabledOnly = false;

await graphClient.Groups["{group-id}"]
    .GetMemberGroups(securityEnabledOnly)
    .Request()
    .PostAsync();

```