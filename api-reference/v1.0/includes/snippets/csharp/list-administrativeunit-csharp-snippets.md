---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d747ea01c84b370088e88beba20d61b384839eb5
ms.sourcegitcommit: b8b0e88b3ba9a434dc45f5ab640cb46f66fae299
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/13/2021
ms.locfileid: "52474851"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var administrativeUnit = await graphClient.Education.Classes["{educationClass-id}"].Members["{educationUser-id}"].Schools["{educationSchool-id}"].AdministrativeUnit
    .Request()
    .GetAsync();

```