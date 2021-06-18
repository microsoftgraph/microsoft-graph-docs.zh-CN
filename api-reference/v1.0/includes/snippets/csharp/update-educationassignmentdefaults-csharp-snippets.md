---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 89f428d00dfea81ae0ee281483d5bdce1ecc26b6
ms.sourcegitcommit: 979fe005c74eb99cd971df6b9511b2d3f7fe3cd4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/17/2021
ms.locfileid: "52991022"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var educationAssignmentDefaults = new EducationAssignmentDefaults
{
    AddedStudentAction = EducationAddedStudentAction.AssignIfOpen,
    NotificationChannelUrl = "https://graph.microsoft.com/beta/teams('acdefc6b-2dc6-4e71-b1e9-6d9810ab1793')/channels('3da03fc4-8eac-4459-84fb-1422dc01f65e')"
};

await graphClient.Education.Classes["{educationClass-id}"].AssignmentDefaults
    .Request()
    .UpdateAsync(educationAssignmentDefaults);

```