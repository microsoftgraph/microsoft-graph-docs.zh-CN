---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 436596366abc45da1cd02c0f57d6f60ab137bf732ed55277c63537f6a0dd4349
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57328692"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var installedApps = await graphClient.Users["{user-id}"].Teamwork.InstalledApps
    .Request()
    .Filter("teamsApp/externalId eq 'cf1ba4c7-f94e-4d80-ba90-5594b641a8ee'")
    .Expand("teamsAppDefinition")
    .GetAsync();

```