---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4f3b40fb2647b8b9c9f59530c764c1481f7a544678d6aebca7cc95e7c71b0ed6
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57332087"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Education.Classes["{educationClass-id}"].Assignments["{educationAssignment-id}"].Categories["{educationCategory-id}"].Reference
    .Request()
    .DeleteAsync();

```