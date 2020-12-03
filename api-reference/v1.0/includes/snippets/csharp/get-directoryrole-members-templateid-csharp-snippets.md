---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3399e1bf270847044f41025385673577a716f69b
ms.sourcegitcommit: 9f88b7e41a4a4a4d5f52bd995ce07c6f702bd5d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/01/2020
ms.locfileid: "49524568"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var members = await graphClient.DirectoryRoles["roleTemplateId=4a5d8f65-41da-4de4-8968-e035b65339cf"].Members
    .Request()
    .GetAsync();

```