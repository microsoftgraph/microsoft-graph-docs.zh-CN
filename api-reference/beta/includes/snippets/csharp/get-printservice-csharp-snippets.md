---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1e9a7a2066d32dfd4066c0ad8deb6999f777773a
ms.sourcegitcommit: 9edfcf99706c8490cd5832a1c706a88a89e24db1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/07/2020
ms.locfileid: "42947550"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var printService = await graphClient.Print.Services["{id}"]
    .Request()
    .GetAsync();

```