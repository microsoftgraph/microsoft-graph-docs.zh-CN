---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d391d329cad64d627717d724d6961d7d2e84475d
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2021
ms.locfileid: "50470366"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var educationAssignmentResource = new EducationAssignmentResource
{
    DistributeForStudentWork = false
};

await graphClient.Education.Classes["11021"].Assignments["19002"].Resources["850f51b7-1df9-4ec0-bd62-64a0214b9cbf"]
    .Request()
    .UpdateAsync(educationAssignmentResource);

```