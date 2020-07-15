---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 97e8be988d6e09b17b0d5cf250e01cc792fdd678
ms.sourcegitcommit: 2c8a12389b82ee5101b2bd17eae11b42e65e52c0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/15/2020
ms.locfileid: "45142345"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var displayName = "Contoso IWA App";

await graphClient.ApplicationTemplates["8adf8e6e-67b2-4cf2-a259-e3dc5476c621"]
    .Instantiate(displayName)
    .Request()
    .PostAsync();

```