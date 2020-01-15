---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 555a6fff3df8a69a835ae7d54cc005e9c3953096
ms.sourcegitcommit: 5f643d3b3f71a9711963c8953da2188539fc9b0c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/14/2020
ms.locfileid: "41123104"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var tasks = await graphClient.Planner.Buckets["{bucket-id}"].Tasks
    .Request()
    .GetAsync();

```