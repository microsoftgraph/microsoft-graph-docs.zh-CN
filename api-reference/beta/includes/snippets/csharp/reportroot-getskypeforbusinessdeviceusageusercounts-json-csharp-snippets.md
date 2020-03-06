---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0ddc68e742fd178ec9647e05e3ec5c17c6685c3d
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36359472"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getSkypeForBusinessDeviceUsageUserCounts = await graphClient.Reports
    .GetSkypeForBusinessDeviceUsageUserCounts("D7")
    .Request()
    .GetAsync();

```