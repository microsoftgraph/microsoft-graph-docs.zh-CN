---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 0c7f64f29df73c68ff0502973155fe3f9d72593f
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36360182"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getOneDriveActivityUserDetail = await graphClient.Reports
    .GetOneDriveActivityUserDetail("D7")
    .Request()
    .GetAsync();

```