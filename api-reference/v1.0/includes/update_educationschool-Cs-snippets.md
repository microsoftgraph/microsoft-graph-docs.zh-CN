---
description: 自动生成的文件。 不修改
ms.openlocfilehash: ba842a052edfb19e5f7333912aa979a91a704003
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34453423"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var educationSchool = new EducationSchool
{
    DisplayName = "Fabrikam Arts High School",
    Description = "Magnate school for the arts. Los Angeles School District"
};

await graphClient.Education.Schools["{school-id}"]
    .Request()
    .UpdateAsync(educationSchool);

```