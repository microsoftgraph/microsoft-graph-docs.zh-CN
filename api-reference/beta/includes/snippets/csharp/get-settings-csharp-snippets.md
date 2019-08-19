---
description: 自动生成的文件。 不修改
ms.openlocfilehash: bcf2609b6e1da776feb4416deec9ffa98b916bcb
ms.sourcegitcommit: f50b1feff72182d1e19bfa346304beaf29558b68
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/19/2019
ms.locfileid: "36461559"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var analytics = await graphClient.Me.Analytics
    .Request()
    .Select( e => new {
             e.Settings 
             })
    .GetAsync();

var settings = analytics.Settings;

```