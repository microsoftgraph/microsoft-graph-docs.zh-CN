---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6172bb5f0d20d5b576b58796ad7dd85862f061df
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2021
ms.locfileid: "50472190"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var educationAssignment = await graphClient.Education.Classes["11014"].Assignments["19002"]
    .Request()
    .GetAsync();

```