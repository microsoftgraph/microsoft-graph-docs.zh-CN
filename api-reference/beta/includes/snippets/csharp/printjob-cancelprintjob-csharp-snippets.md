---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 76cb1411e08472adc5b8bbb2bf2a031d9c0db706
ms.sourcegitcommit: 9edfcf99706c8490cd5832a1c706a88a89e24db1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/07/2020
ms.locfileid: "42947559"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Print.Printers["{id}"].Jobs["{id}"]
    .CancelPrintJob()
    .Request()
    .PostAsync();

```