---
description: 自动生成的文件。 不修改
ms.openlocfilehash: f0d7b1f5b104ce0c8899d48dc22288f56452ee2d
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35892970"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var supportedTimeZones = await graphClient.Me.Outlook
    .SupportedTimeZones(microsoft.graph.timeZoneStandard'Iana')
    .Request()
    .GetAsync();

```