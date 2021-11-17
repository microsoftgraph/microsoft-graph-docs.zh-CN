---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ce7001fd5878333da5f2fefe02a9ff137b0bdf0b8cf67bfc543a3b7f3ef2bc1b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57164055"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Users["{user-id}"].Teamwork.InstalledApps["{userScopeTeamsAppInstallation-id}"]
    .Request()
    .DeleteAsync();

```