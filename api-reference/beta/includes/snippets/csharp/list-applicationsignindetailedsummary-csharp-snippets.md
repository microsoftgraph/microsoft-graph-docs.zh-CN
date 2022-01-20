---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 45246cd1e3d9ec171953dffc31d7c5647bd6f049
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62096107"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var applicationSignInDetailedSummary = await graphClient.Reports.ApplicationSignInDetailedSummary
    .Request()
    .GetAsync();

```