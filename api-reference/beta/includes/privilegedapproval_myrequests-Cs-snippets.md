---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 839b860f5ac22250a3811413b929d91f8322386a
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34443262"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var myRequests = await graphClient.PrivilegedApproval.MyRequests()
    .Request()
    .GetAsync();

```