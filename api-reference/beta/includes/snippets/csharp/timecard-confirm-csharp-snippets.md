---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3c199f5fcda88ca9207bf7ccc0031e4d3035e975c4229d9ffeca6d43e32885ff
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57106486"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Teams["{team-id}"].Schedule.TimeCards["{timeCard-id}"]
    .Confirm()
    .Request()
    .PostAsync();

```