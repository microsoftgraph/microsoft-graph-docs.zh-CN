---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 28fdd51600c5bf43b0889ba0a775b0a8186f460b097e0d3b2ee2e11b52df3a36
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57161480"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var submissions = await graphClient.Education.Classes["{educationClass-id}"].Assignments["{educationAssignment-id}"].Submissions
    .Request()
    .GetAsync();

```