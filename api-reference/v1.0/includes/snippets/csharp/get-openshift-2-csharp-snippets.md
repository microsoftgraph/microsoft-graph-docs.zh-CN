---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8f3a6d7089c7cf8d9bcdcf583e67e1d008afa07b80115a0d143509895ad12f05
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57162567"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var openShifts = await graphClient.Teams["{team-id}"].Schedule.OpenShifts
    .Request()
    .GetAsync();

```