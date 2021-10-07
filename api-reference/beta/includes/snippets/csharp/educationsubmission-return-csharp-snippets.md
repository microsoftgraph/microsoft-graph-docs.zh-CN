---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6ddf88b2e18b8dba3bcba296cec0d3c9a17c849baf60c851323ddb1cf4136bfe
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57162254"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Education.Classes["{educationClass-id}"].Assignments["{educationAssignment-id}"].Submissions["{educationSubmission-id}"]
    .Return()
    .Request()
    .PostAsync();

```