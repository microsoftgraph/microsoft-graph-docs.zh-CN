---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 343b02c7aad7ca6524c8f026a06f06fe0b9cdbb6
ms.sourcegitcommit: 36bae3615df41876493b25da478e589d1974f97b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/29/2021
ms.locfileid: "59996169"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Education.Classes["{educationClass-id}"].Assignments["{educationAssignment-id}"].Submissions["{educationSubmission-id}"]
    .Reassign()
    .Request()
    .PostAsync();

```