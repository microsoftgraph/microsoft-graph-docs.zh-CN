---
description: 自动生成的文件。 不修改
ms.openlocfilehash: ddabb21e62ba3dd90cb6ab215fe826b11e02ee89
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35479624"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.AdministrativeUnits["{id}"].ScopedRoleMembers["{id}"]
    .Request()
    .DeleteAsync();

```