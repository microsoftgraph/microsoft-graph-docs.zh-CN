---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6bbc37dd7ac2faf78dcd5d0f661f4237d00de85d723a27408407b9ebc4fc71c1
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57105718"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Teams["{team-id}"].Schedule.Shifts["{shift-id}"]
    .Request()
    .DeleteAsync();

```