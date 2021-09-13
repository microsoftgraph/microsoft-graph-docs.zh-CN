---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9c5963c6ab2f8e98ecaeec7f69f759fa9700b4af138b65c8e44633ee3e4a5964
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57220117"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var installedApps = await graphClient.Users["{user-id}"].Teamwork.InstalledApps
    .Request()
    .Expand("teamsAppDefinition")
    .GetAsync();

```