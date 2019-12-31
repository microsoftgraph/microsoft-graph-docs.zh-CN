---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 11dbab6d04a2f95e8117a5fe425deda9b0fd6238
ms.sourcegitcommit: 636671293b0be89088459c4fc8a5e661341b37cf
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/31/2019
ms.locfileid: "40912917"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var clientContext = "clientContext-value";

await graphClient.Communications.Calls["{id}"]
    .CancelMediaProcessing(clientContext)
    .Request()
    .PostAsync();

```