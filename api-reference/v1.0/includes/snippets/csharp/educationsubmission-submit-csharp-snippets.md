---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 27785b825a280f5d14ceb63d344cfd36d33705e56d265a9727f29a40d6a0d08e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57332074"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Education.Classes["{educationClass-id}"].Assignments["{educationAssignment-id}"].Submissions["{educationSubmission-id}"]
    .Submit()
    .Request()
    .PostAsync();

```