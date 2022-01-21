---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 343b02c7aad7ca6524c8f026a06f06fe0b9cdbb6
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62111188"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Education.Classes["{educationClass-id}"].Assignments["{educationAssignment-id}"].Submissions["{educationSubmission-id}"]
    .Reassign()
    .Request()
    .PostAsync();

```