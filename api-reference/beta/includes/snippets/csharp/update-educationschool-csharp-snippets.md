---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6b13da3d6a9f01d5c4619ec283b676c05c0bd0236b4689f72d1446b1d2aed182
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57332918"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var educationSchool = new EducationSchool
{
    DisplayName = "Fabrikam Arts High School",
    Description = "Magnate school for the arts. Los Angeles School District"
};

await graphClient.Education.Schools["{educationSchool-id}"]
    .Request()
    .UpdateAsync(educationSchool);

```