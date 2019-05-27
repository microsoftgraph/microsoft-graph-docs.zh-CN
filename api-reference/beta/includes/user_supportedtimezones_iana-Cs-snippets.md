---
description: 自动生成的文件。 不修改
ms.openlocfilehash: cfda948bf615e89610f1d1db5ed2daf54ed5cacc
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34456601"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var supportedTimeZones = await graphClient.Me.Outlook.SupportedTimeZones(microsoft.graph.timeZoneStandard'Iana')
    .Request()
    .GetAsync();

```