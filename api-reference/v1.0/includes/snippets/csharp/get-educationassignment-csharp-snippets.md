---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ea1f6c766289c261fc919631c09cba521b908e7d0c30d8dfcf8c742474f64437
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57378259"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var educationAssignment = await graphClient.Education.Classes["{educationClass-id}"].Assignments["{educationAssignment-id}"]
    .Request()
    .GetAsync();

```