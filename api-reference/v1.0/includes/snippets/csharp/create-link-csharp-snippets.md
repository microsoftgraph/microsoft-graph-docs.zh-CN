---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: aa297e12793bb6d9e58e59bf7268a533942484b2
ms.sourcegitcommit: 5575e6607817ba23ceb0b01e2f5fc81e58bdcd1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/22/2020
ms.locfileid: "43771054"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var type = "view";

var scope = "anonymous";

await graphClient.Me.Drive.Items["{item-id}"]
    .CreateLink(type,scope,null,null,null)
    .Request()
    .PostAsync();

```