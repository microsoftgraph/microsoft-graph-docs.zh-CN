---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 76f36a3dee42a6fb5619e25c551f3e48ffec8393
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35520793"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var Participant = await graphClient.App.Calls["{id}"].Participants["{id}"]
    .Request()
    .GetAsync();

```