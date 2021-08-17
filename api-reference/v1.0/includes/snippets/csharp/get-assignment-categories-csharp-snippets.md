---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5034c4439542e876c6ba93e682f72341324e7abeaf10ba9a9e65e1e9e5426fa6
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57378258"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var categories = await graphClient.Education.Classes["{educationClass-id}"].Assignments["{educationAssignment-id}"].Categories
    .Request()
    .GetAsync();

```