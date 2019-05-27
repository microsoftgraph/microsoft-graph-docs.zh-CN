---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 8cddd844439f86ba66ecf43c9ec10f2e3a6ebe05
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34470139"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var versions = await graphClient.Me.Drive.Items["{item-id}"].Versions["{version-id}"]
    .Request()
    .Select( e => new {
             e.Content 
             })
    .GetAsync();

var content = versions.Content;

```