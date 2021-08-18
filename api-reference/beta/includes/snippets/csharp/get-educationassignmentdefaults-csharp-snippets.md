---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 206c21573440287a78c4455aeb8659c309b704b7929afe006b3910a717df7daf
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57332919"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var educationAssignmentDefaults = await graphClient.Education.Classes["{educationClass-id}"].AssignmentDefaults
    .Request()
    .GetAsync();

```