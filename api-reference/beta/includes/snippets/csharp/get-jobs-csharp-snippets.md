---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6e9b795a0d36eee98985c0c056cf03066eec43af
ms.sourcegitcommit: 6ec748ef00d025ee216274a608291be3c1257777
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/27/2021
ms.locfileid: "50015380"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var jobs = await graphClient.Print.Printers["{id}"].Jobs
    .Request()
    .GetAsync();

```