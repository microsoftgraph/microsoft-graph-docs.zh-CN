---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 0f0de65547b6beba04649ea5058fde1aef706934
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35509775"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var memberOf = await graphClient.Devices["{id}"].MemberOf
    .Request()
    .GetAsync();

```