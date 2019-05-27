---
description: 自动生成的文件。 不修改
ms.openlocfilehash: b226f87522412109ff3163236b5a0554adb40105
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34479572"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var educationSchool = await graphClient.Education.Schools["{school-id}"]
    .Request()
    .GetAsync();

```