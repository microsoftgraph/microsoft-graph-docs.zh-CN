---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 919ab665a2ff2917c8dc8dfac7c27b487a0b5baa
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50808716"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Education.Classes["{educationClass-id}"].Assignments["{educationAssignment-id}"].Submissions["{educationSubmission-id}"]
    .Return()
    .Request()
    .PostAsync();

```