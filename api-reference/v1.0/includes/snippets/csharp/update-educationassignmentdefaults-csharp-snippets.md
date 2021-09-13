---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 80b543054afade04af15bc83d767c660937c493923d8bfc0e4fc9ffde2096abb
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57333970"
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