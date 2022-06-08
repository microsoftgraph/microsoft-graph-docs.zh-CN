---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4f8be6b4ef93875a19ed23a615be0ab1c13a6532
ms.sourcegitcommit: a345f96fb22115f65840702a4acf0acc7c1b0679
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/08/2022
ms.locfileid: "65946803"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var user = await graphClient.Users["{user-id}"]
    .Request()
    .Select("ext55gb1l09_msLearnCourses")
    .GetAsync();

```