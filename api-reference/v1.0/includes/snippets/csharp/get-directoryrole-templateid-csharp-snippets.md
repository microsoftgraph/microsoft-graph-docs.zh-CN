---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f21e9096525910f4fe4c05e1d7a7fd030259bc0f
ms.sourcegitcommit: 9f88b7e41a4a4a4d5f52bd995ce07c6f702bd5d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/01/2020
ms.locfileid: "49522724"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var directoryRole = await graphClient.DirectoryRoles["roleTemplateId=4a5d8f65-41da-4de4-8968-e035b65339cf"]
    .Request()
    .GetAsync();

```