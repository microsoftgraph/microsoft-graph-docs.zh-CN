---
description: 自动生成的文件。 不修改
ms.openlocfilehash: d5a329ab9cfbfb9070657d1817d3777dec59f1e5
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36358424"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getYammerDeviceUsageUserDetail = await graphClient.Reports
    .GetYammerDeviceUsageUserDetail("D7")
    .Request()
    .GetAsync();

```