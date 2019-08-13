---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 3f0e6d9142c80ad570def8433d0376382791753a
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36320259"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var report = await graphClient.Reports
    .GetYammerDeviceUsageUserDetail("D7")
    .Request()
    .GetAsync();

```