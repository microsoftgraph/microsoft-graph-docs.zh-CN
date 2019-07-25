---
description: 自动生成的文件。 不修改
ms.openlocfilehash: c472d91e50fd8119f2daa03a7a8273404489f8de
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35867703"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var findRooms = await graphClient.Me
    .FindRooms()
    .Request()
    .GetAsync();

```