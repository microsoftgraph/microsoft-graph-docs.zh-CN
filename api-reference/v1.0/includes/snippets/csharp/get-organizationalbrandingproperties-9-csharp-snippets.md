---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f70490b6c791ba1f187fd2e269b770c84939db458c6abcdadeb94579f6ecd6ea
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57329086"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var localizations = await graphClient.Organization["{organization-id}"].Branding.Localizations
    .Request()
    .GetAsync();

```