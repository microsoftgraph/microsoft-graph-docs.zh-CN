---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 629c24d18e30401626f1b562fa85e434f9764fdb
ms.sourcegitcommit: 91d8454bfff853905e3a5e86623fcb06931507ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/03/2021
ms.locfileid: "52870120"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Education.Classes["{educationClass-id}"].Assignments["{educationAssignment-id}"].Submissions["{educationSubmission-id}"]
    .SetUpResourcesFolder()
    .Request()
    .PostAsync();

```