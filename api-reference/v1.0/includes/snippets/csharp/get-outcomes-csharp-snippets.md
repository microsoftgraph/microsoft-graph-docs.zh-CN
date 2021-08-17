---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0379e74b9c3e57d59bbe7bb670db260e73a5f9c9bbd7640a1f268d130b8b58ce
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57333511"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var outcomes = await graphClient.Education.Classes["{educationClass-id}"].Assignments["{educationAssignment-id}"].Submissions["{educationSubmission-id}"].Outcomes
    .Request()
    .GetAsync();

```