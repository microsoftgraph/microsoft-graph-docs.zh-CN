---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a1a9379debfefd8531eade987c6bf408665d7abde8bba30087d302dbd5d2e154
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57409733"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Education.Classes["{educationClass-id}"].Assignments["{educationAssignment-id}"].Submissions["{educationSubmission-id}"]
    .SetUpResourcesFolder()
    .Request()
    .PostAsync();

```