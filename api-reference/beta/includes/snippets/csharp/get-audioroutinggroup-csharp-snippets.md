---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6133f0354356a0d40e834c7b271e446ab42f10f5
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50788128"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var audioRoutingGroup = await graphClient.Communications.Calls["{call-id}"].AudioRoutingGroups["{audioRoutingGroup-id}"]
    .Request()
    .GetAsync();

```