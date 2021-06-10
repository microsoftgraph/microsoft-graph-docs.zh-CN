---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c34ea529dc03913b93dc9d23be973574ba9bd5c8
ms.sourcegitcommit: 503c72036c376a30e08c29df8e7730a7afcab66e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/10/2021
ms.locfileid: "52869854"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var printUsageByUser = await graphClient.Print.Reports.DailyPrintUsageByUser["{printUsageByUser-id}"]
    .Request()
    .GetAsync();

```