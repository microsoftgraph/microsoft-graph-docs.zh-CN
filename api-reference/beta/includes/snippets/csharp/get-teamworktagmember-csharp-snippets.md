---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f787b42fa77fe7d417f4b8415399f3fb18394fdb312d1c23bf208d46fb4fc16e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57163915"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var teamworkTagMember = await graphClient.Teams["{team-id}"].Tags["{teamworkTag-id}"].Members["{teamworkTagMember-id}"]
    .Request()
    .GetAsync();

```