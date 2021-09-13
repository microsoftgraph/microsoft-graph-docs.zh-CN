---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5e203c196a1f172f8899820b43251ff34bd9cdacdea0a9e119b9407ed3c7a67d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57378689"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var installedApps = await graphClient.Teams["{team-id}"].InstalledApps
    .Request()
    .GetAsync();

```