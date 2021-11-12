---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c64048ef880aabc3492e63a4f4ff578ebe80c27e79854763f08259a507ea1c27
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57162914"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var educationCategory = new EducationCategory
{
    DisplayName = "Quizzes"
};

await graphClient.Education.Classes["{educationClass-id}"].AssignmentCategories
    .Request()
    .AddAsync(educationCategory);

```