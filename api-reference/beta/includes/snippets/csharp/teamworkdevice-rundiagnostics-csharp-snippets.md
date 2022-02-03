---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 826f157ac857d56f2df745c60698f239111bb107
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62347879"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Teamwork.Devices["{teamworkDevice-id}"]
    .RunDiagnostics()
    .Request()
    .PostAsync();

```