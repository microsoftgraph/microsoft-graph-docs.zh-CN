---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1b77e9daf386992c3fe33411d628140d707c21e5
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/30/2021
ms.locfileid: "53211911"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Education.Classes["{educationClass-id}"].Assignments["{educationAssignment-id}"].Categories["{educationCategory-id}"].Reference
    .Request()
    .DeleteAsync();

```