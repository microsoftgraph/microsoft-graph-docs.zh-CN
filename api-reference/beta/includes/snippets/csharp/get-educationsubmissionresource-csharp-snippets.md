---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d6f466fecf3eaa32689a16913eebd97fe62453d8
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50800955"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var educationSubmissionResource = await graphClient.Education.Classes["{educationClass-id}"].Assignments["{educationAssignment-id}"].Submissions["{educationSubmission-id}"].Resources["{educationSubmissionResource-id}"]
    .Request()
    .GetAsync();

```