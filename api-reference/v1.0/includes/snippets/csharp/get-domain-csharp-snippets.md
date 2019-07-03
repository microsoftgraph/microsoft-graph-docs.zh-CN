---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 4bf9214aaf694fc1ebfb4a87423825ea72cab649
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35463017"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var domain = await graphClient.Domains["contoso.com"]
    .Request()
    .GetAsync();

```