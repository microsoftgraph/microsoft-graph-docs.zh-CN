---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 576455c14e1235b36842631d076f0d76aac5eefd
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35492841"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var educationClass = await graphClient.Education.Classes["{class-id}"]
    .Request()
    .GetAsync();

```