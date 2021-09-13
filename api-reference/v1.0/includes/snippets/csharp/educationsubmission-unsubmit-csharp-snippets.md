---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3776ee35d6717cb73b3cc28ed656987e6f88bbeb7ba9384045e88457a3ac2008
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57274254"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Education.Classes["{educationClass-id}"].Assignments["{educationAssignment-id}"].Submissions["{educationSubmission-id}"]
    .Unsubmit()
    .Request()
    .PostAsync();

```