---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 97c797be70a287b963b7ed5d93ba956bf4e0e3e69159b82a9c36aac1ceafb433
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57219766"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var educationAssignmentSettings = new EducationAssignmentSettings
{
    SubmissionAnimationDisabled = true
};

await graphClient.Education.Classes["{educationClass-id}"].AssignmentSettings
    .Request()
    .UpdateAsync(educationAssignmentSettings);

```