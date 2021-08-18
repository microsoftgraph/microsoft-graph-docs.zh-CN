---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9096f40167745ab6151b53f6117a3f3016bf68f77704b15064c15c26471f7f27
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57278704"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var educationAssignmentResource = await graphClient.Education.Classes["{educationClass-id}"].Assignments["{educationAssignment-id}"].Resources["{educationAssignmentResource-id}"]
    .Request()
    .GetAsync();

```